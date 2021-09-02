# `setup-scala-util` GitHub Action

A GitHub Action to add Scala utilities to the PATH.

Utilities
=========

* `sbt-const` - Extract the string literal from a `val` or `def` field in your sbt build.

  Example:

  ```sh
  > grep 'val scala.*=' project/*.scala
  project/Dependencies.scala:    val scala2          = "2.13.6"
  project/Dependencies.scala:    val scala3          = "3.0.2"
  project/Dependencies.scala:    val scalaJsDom      = "1.2.0"
  project/Dependencies.scala:    val scalaJsReact    = "2.0.0-RC2"
  project/Dependencies.scala:    val scalaJsJavaTime = "1.0.0"

  > sbt-const scala2
  2.13.6
  ```
