# Quickstart

Let's get Solr up an running. To start Solr, we'll run the `start.jar` file from the example folder of our Solr installation. A fully preconfigured demo installation of Solr is also in the example folder. We'll work with this demo installation throughout this tutorial.

To start the demo server, change your directory to the example folder and run this command:

```
java -jar start.jar
```

This will launch a [Jetty](http://en.wikipedia.org/wiki/Jetty_(web_server)) server on your computer which will be running Java. The window which you ran the command in will become a scrolling logfile, and should look something like this:

```
...
2829 [main] INFO  org.eclipse.jetty.server.AbstractConnector  – Started SocketConnector@0.0.0.0:8983
2840 [searcherExecutor-5-thread-1] INFO  org.apache.solr.core.SolrCore  – [collection1] webapp=null path=null params={event=firstSearcher&q=static+firstSearcher+warming+in+solrconfig.xml&distrib=false} hits=0 status=0 QTime=40 
2840 [searcherExecutor-5-thread-1] INFO  org.apache.solr.core.SolrCore  – QuerySenderListener done.
2840 [searcherExecutor-5-thread-1] INFO  org.apache.solr.handler.component.SpellCheckComponent  – Loading spell index for spellchecker: default
2841 [searcherExecutor-5-thread-1] INFO  org.apache.solr.handler.component.SpellCheckComponent  – Loading spell index for spellchecker: wordbreak
2841 [searcherExecutor-5-thread-1] INFO  org.apache.solr.handler.component.SuggestComponent  – Loading suggester index for: mySuggester
2841 [searcherExecutor-5-thread-1] INFO  org.apache.solr.spelling.suggest.SolrSuggester  – reload()
2841 [searcherExecutor-5-thread-1] INFO  org.apache.solr.spelling.suggest.SolrSuggester  – build()
2850 [searcherExecutor-5-thread-1] INFO  org.apache.solr.core.SolrCore  – [collection1] Registered new searcher Searcher@6e72814f[collection1] main{StandardDirectoryReader(segments_1:1:nrt)}
```

If everything is working correctly, you should be able to see the adminstrative interface at [http://localhost:8983/solr/](http://localhost:8983/solr/)

You can poke around the adminstrative site, but there isn't any data there yet, so there's not much to see. So let's shut the server down by going to the command line window with the scolling server log and hitting `Ctrl+c`. You should see a few messages at the end of the log about the server stopping, then the command line will return.

This is a good time to point out that Solr provides absolutely no security. If you were to run Solr on a server connected to the Web, anyone would be able to visit your Solr installation at https://example.org:8983/solr/ and be able to tinker with your data, and even delete it. It's up to you to control access to Solr via your server configuration.

[Next]() or [Back]() or [Home]()
