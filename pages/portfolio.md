---
layout: empty
title: "Portfolio"
date: 2018-10-18
description: |
  Zerocracy solves a number of problems we
  all experience in software development projects,
  and helps optimize costs and increase quality.
permalink: portfolio.html
no_disqus: true
hidden: true
projects:
  takes:
    name: Takes
    href: https://www.takes.org/
    logo: https://www.takes.org/clapper.jpg
    width: 64
    license: MIT
    sources: https://github.com/yegor256/takes
    stack: Java, XML, XSLT, Velocity
    loc: ?
    hoc: ?
    team: 7
    start: 2015/Feb
    case: |
      True Object-Oriented and Immutable Java Web Development Framework,
      a replacement of outdated SpringMVC and Play, read this blog post:
      [Java Web App Architecture In Takes Framework](http://www.yegor256.com/2015/03/22/takes-java-web-framework.html)
  cactoos:
    name: Cactoos
    href: https://www.cactoos.org/
    logo: https://www.cactoos.org/logo.svg
    width: 64
    license: MIT
    sources: https://github.com/yegor256/cactoos
    stack: Java, OOP
    loc: ?
    hoc: ?
    team: 15
    start: 2017/May
    case: |
      Object-Oriented library of Java primitives, an alternative
      to Google Guava and Apache Commons, making code more elegant
      and cleaer, according to the principles of [Elegant Objects](https://www.elegantobjects.org).
  rultor:
    name: Rultor
    href: http://www.rultor.com/
    logo: http://doc.rultor.com/images/logo.svg
    width: 64
    license: BSD
    sources: https://github.com/yegor256/rultor
    stack: Java, Docker, DynamoDB, Bash, Git, Github API, Maven, CasperJS, SASS, PostgreSQL
    loc: 12.7K
    hoc: 427K
    team: 12
    start: 2013/Jun
    lifetime: 18
    case: |
      Coding team assistant, automating merge, release, and deploy operations. It
      exploits Docker containers for builds isolation. Read some articles
      about it: [Every Build in Its Own Docker Container](http://www.yegor256.com/2014/07/29/docker-in-rultor.html),
      [Rultor + Travis](http://www.yegor256.com/2014/07/31/travis-and-rultor.html) and
      [Rultor, a Merging Bot](http://www.yegor256.com/2014/07/24/rultor-automated-merging.html)
  zold:
    name: Zold
    href: https://www.zold.io/
    logo: https://www.zold.io/logo.png
    width: 64
    license: MIT
    sources: https://github.com/zold-io/zold
    stack: Ruby, Sinatra, XML, Cryptocurrency
    loc: ?
    hoc: ?
    team: 8
    start: 2018/Jan
    case: |
      An experimental cryptocurrency for fast micro payments,
      based on the proof-of-work principle, but without the Blockchain. More
      information about it at the [White Paper](https://papers.zold.io/wp.pdf).
      There is also a [blog](https://blog.zold.io), where regularly posts new articles.
  jcabi.com:
    name: JCabi
    href: http://www.jcabi.com/
    logo: http://img.jcabi.com/logo-square.svg
    width: 64
    license: BSD
    sources: https://github.com/jcabi/jcabi
    stack: Java, MySQL, Heroku, Elastic Beanstalk, S3, DynamoDB, SimpleDB, Github API, Maven plugins, HTTP, JUnit, Hamcrest
    loc: 97.2K
    hoc: 499K
    team: 27
    start: 2012/Apr
    case: |
      Useful Java components, including AOP aspects, DynamoDB SDK, MySQL Maven Plugin, etc.
      Check these articles about the most interesting jcabi components:
      [Fluent Java Http Client](http://www.yegor256.com/2014/04/11/jcabi-http-intro.html),
      [Object-Oriented Github API](http://www.yegor256.com/2014/05/14/object-oriented-github-java-sdk.html),
      [MySQL Maven Plugin](http://www.yegor256.com/2014/05/21/mysql-maven-plugin.html), and
      [Object-Oriented DynamoDB API](http://www.yegor256.com/2014/04/14/jcabi-dynamo-java-api-of-aws-dynamodb.html).
  tacit:
    name: Tacit
    href: https://github.com/yegor256/tacit
    logo: https://github.com/yegor256/tacit/raw/master/tacit_logo.png
    width: 64
    license: MIT
    sources: https://github.com/yegor256/tacit
    stack: CSS, HTML
    loc: ?
    hoc: ?
    team: 8
    start: 2015/Apr
    case: |
      CSS framework without a single
      "class," especially for those who don't understand anything in graphic
      design, but want their websites to look attractive, announced in
      [this blog post](https://www.yegor256.com/2015/apr/2015-04-13-tacit-css-framework-for-dummies.html).
  stateful.co:
    name: Stateful
    href: http://www.stateful.co/
    logo: http://img.stateful.co/pomegranate.svg
    width: 64
    license: BSD
    sources: https://github.com/sttc/stateful
    stack: Java, DynamoDB, Maven, JUnit, CasperJS, Bootstrap, SASS
    loc: 8.7K
    hoc: 10.4K
    team: 3
    start: 2014/May
    lifetime: 6
    case: |
      Stateful RESTful web privitives with XML/JSON API. We are actively
      using this web tool in every application that works with DynamoDB.
      [Atomic Counters at Stateful.co](http://www.yegor256.com/2014/05/18/cloud-autoincrement-counters.html)
      article explain the details.
  s3auth:
    name: S3Auth
    href: http://www.s3auth.com
    logo: http://img.s3auth.com/logo.svg
    width: 128
    license: BSD
    sources: https://github.com/yegor256/s3auth
    stack: Java, DynamoDB, S3, EC2, H2 Database, Maven, JUnit, Mockito, XML/XSLT, HTML5, CSS
    loc: 12.3K
    hoc: 42.8K
    team: 3
    start: 2012/Aug
    lifetime: 35
    case: |
      s3auth.com is a gateway to private AWS S3 buckets that
      provides Basic HTTP authentication. At the moment, s3auth.com
      hosts over 300 domains and sends through more than 10Mb of data each hour.
      [This blog post](http://www.yegor256.com/2014/04/21/s3-http-basic-auth.html)
      explains its business case with more details.
  netbout:
    name: Netbout
    href: http://www.netbout.com/
    logo: http://img.netbout.com/logo.svg
    width: 128
    license: BSD
    sources: https://github.com/yegor256/netbout
    stack: Java, DynamoDB, H2 Database, Maven, JUnit, Mockito, XML/XSLT, HTML5, CSS, jQuery
    loc: 13.9K
    hoc: 732K
    team: 8
    start: 2010/Apr
    lifetime: 57
    case: |
      Secure online environment for private
      long-term business communications. Originally developed in PHP,
      then migrated to Java, then re-factored and simplified. At the moment,
      it is actively used in our internal communications.
  qulice:
    name: Qulice
    href: http://www.qulice.com/
    logo: http://img.qulice.com/logo.svg
    width: 150
    license: BSD
    sources: https://github.com/teamed/qulice
    stack: Java, Maven plugins, Checkstyle, PMD, FindBugs, JUnit, Mockito
    loc: 10.9K
    hoc: 87.3K
    team: 7
    start: 2011/Aug
    lifetime: 90
    case: |
      Static quality analysis toolkit for Java/Maven projects
  requs:
    name: Requs
    href: http://www.requs.org/
    logo: http://img.requs.org/logo.svg
    width: 150
    license: BSD
    sources: https://github.com/teamed/requs
    stack: Java, XSTL, ANTLR4, Maven plugins, JUnit, Mockito, jQuery
    loc: 12.2K
    hoc: 265K
    team: 6
    start: 2010/Mar
    lifetime: 24
    case: |
      Controlled Natural Language (CNL) and Java library
      for formalization of requirements specification.
      [Incremental Requirements With Requs](http://www.yegor256.com/2014/04/26/incremental-requirements-with-requs.html)
      article explains what is it for and how we're using this tool
      in our projects.
  xembly:
    name: Xembly
    href: http://www.xembly.org/
    logo: http://img.xembly.org/logo-256x256.png
    width: 64
    license: BSD
    sources: https://github.com/yegor256/xembly
    stack: Java, XML, DOM
    loc: 5.5K
    hoc: 10.3K
    team: 3
    start: 2013/Jul
    lifetime: 10
    case: |
      XML manipulation language with Java implementation. Its purpose
      is explain in
      [Xembly, an Assembly for XML](http://www.yegor256.com/2014/04/09/xembly-intro.html) article.
      We actively use this library in almost every project.
  pdd gem:
    name: PDD Ruby Gem
    href: https://github.com/teamed/pdd
    logo: https://avatars2.githubusercontent.com/u/24456188
    width: 64
    license: MIT
    sources: https://github.com/teamed/pdd
    stack: Ruby, Cucumber, Minitest, Rubocop
    loc: 1.5K
    hoc: 9.6K
    team: 1
    start: 2014/Aug
    lifetime: 2
    case: |
      Puzzle Driven Development automation tool that
      parses source code files, finds TODO markers and
      builds an XML report. PDD and this tool are explained
      [here](http://www.yegor256.com/2009/03/04/pdd.html).
  phprack:
    name: PHPRack
    href: http://www.phprack.com
    logo: http://img.phprack.com/logo.png
    width: 96
    license: BSD
    sources: https://github.com/yegor256/phprack
    stack: PHP, PHPCS, PHPMD, xdebug, AJAX, jQuery
    loc: 9.1K
    hoc: 39.7K
    team: 9
    start: 2010/Jan
    lifetime: 20
    case: |
      Integration testing framework that allows on-production
      monitoring of a running script application
---
<style>
td, th {
  font-size: .9em;
  line-height: 1.3em;
}
@media all and (max-width: 1024px) {
  table {
    display: none;
  }
}
ul {
  list-style: none;
  margin-left: 0;
}
li {
  margin-bottom: 4em;
}
@media all and (min-width: 1024px) {
  ul {
    display: none;
    list-style: none;
  }
}
.footnotes {
  font-size: .75em;
  line-height: 1.3em;
}
</style>

<header>
  <nav>
    <ul>
      <li>
        <a href="/">
          <img src="https://www.0crat.com/svg/logo.svg" class="logo" alt="Zerocracy logo"/>
        </a>
      </li>
    </ul>
  </nav>
</header>
<section>
  <table>
    <colgroup>
      <col style="width:15%"/>
      <col style="width:3em"/>
      <col style="width:20%"/>
      <col style="width:3em"/>
      <col style="width:3em"/>
      <col style="width:3em"/>
      <col style="width:4em"/>
      <col style="width:30%"/>
    </colgroup>
    <thead>
      <tr>
        <th>Project</th>
        <th></th>
        <th>Tech Stack</th>
        <th class="desk" style="text-align:right">LoC<sup>1</sup><br/>HoC<sup>4</sup></th>
        <th class="desk" style="text-align:right">Team<sup>2</sup></th>
        <th class="desk">Start</th>
        <th class="desk" style="text-align:right">Life<sup>3</sup></th>
        <th>Business Case</th>
      </tr>
    </thead>
    <tbody>
      {% for p in page.projects %}
        <tr>
          <td>
            <div class="bar"></div>
            <a href="{{ p[1].href }}">
              {% if p[1].logo %}
                <img src="{{ p[1].logo }}" style="width:{{ p[1].width }}px;" alt="{{ p[0] }} logo" class="pic"/>
              {% else %}
                {{ p[0] }}
              {% endif %}
            </a>
          </td>
          <td>
            {% if p[1].sources %}
              <a href="{{ p[1].sources }}" title="{{ p[1].license }}">
                <i class="fa fa-2x fa-github"></i></a>
            {% else %}
              {{ p[1].license }}
            {% endif %}
          </td>
          <td>{{ p[1].stack }}</td>
          <td class="desk mono" style="text-align:right">{{ p[1].loc }}<br/>{{ p[1].hoc }}</td>
          <td class="desk mono" style="text-align:right">{{ p[1].team }}</td>
          <td class="desk">{{ p[1].start }}</td>
          <td class="desk mono" style="text-align:right">
            {% if p[1].lifetime %}
              {{ p[1].lifetime }}
            {% else %}
              &mdash;
            {% endif %}
          </td>
          <td>{{ p[1].case | markdownify }}</td>
        </tr>
      {% endfor %}
    </tbody>
  </table>

  <ul>
    {% for p in page.projects %}
      <li>
        <a href="{{ p[1].href }}" class="mobile-logo">
          {% if p[1].logo %}
            <img src="{{ p[1].logo }}" style="width:{{ p[1].width }}px;" alt="{{ p[0] }} logo" class="pic"/>
          {% else %}
            {{ p[0] }}
          {% endif %}
        </a>
        <br/>
        {% if p[1].name %}
          {{ p[1].name }}
        {% endif %}
        <br/>
        [{{ p[1].stack }}]
        {{ p[1].case | markdownify }}
      </li>
    {% endfor %}
  </ul>

  <p class="footnotes">
    <sup><strong>1</strong></sup> LoC stands for "Lines of Code", excluding empty lines and comments,
      calculated using <a href="http://cloc.sourceforge.net/">cloc</a>.
    <sup><strong>2</strong></sup> Team includes only active contributors to the source code and doesn't
      include testers, active users, and documentation writers.
    <sup><strong>3</strong></sup> Even though all projects are actively exploited by its users,
      some of them are not in active development any more. Lifetime means
      the total calendar time of active development by the project team, in weeks.
    <sup><strong>4</strong></sup> HoC stands for "Hits of Code", calculated by
      <a href="https://github.com/teamed/hoc">hoc</a>, as explained in
      <a href="http://www.yegor256.com/2014/11/14/hits-of-code.html">Hits-of-Code Instead of SLoC</a>
  </p>
</section>
