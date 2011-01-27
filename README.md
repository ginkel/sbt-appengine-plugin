Require
=======

 * [sbt][] 0.7.4
 * [Google App Engine SDK][GAE]
 * [JRebel][] optional

[sbt]: http://simple-build-tool.googlecode.com/
[GAE]: http://code.google.com/intl/en/appengine/downloads.html
[JRebel]: http://www.zeroturnaround.com/jrebel/

Usage
=====

export environment variables

    export APPENGINE_HOME=~/appengine-java-sdk-1.4.0
    export JREBEL_HOME=~/jrebel-3.5

Create project/plugins/Plugins.scala

<pre><code>import sbt._

class Plugins(info: ProjectInfo) extends PluginDefinition(info) {
  val appenginePlugin = "net.stbbs.yasushi" % "sbt-appengine-plugin" % "2.3-SNAPSHOT"
}
</code></pre>

----
[Hello World example][HelloWorld]

[HelloWorld]: http://gist.github.com/377611
