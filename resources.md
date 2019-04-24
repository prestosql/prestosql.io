---
layout: page
menu_id: resources
title: Resources
---

<div class="leftcol widecol faq">

    <h2 id="odbc">Presto ODBC</h2>

    <p>
        There are drivers available from:
        <a href="#prestogres">Prestogres</a>,
        <a href="#starburst">Starburst Data</a>
    </p>

    <h3 id="prestogres">Prestogres</h3>

    <div class="item">
        <h4>Prestogres</h4>
        <dl>
            <dt>Project</dt>
            <dd><a href="https://github.com/treasure-data/prestogres">GitHub</a></dd>
            <dt>Maintained by</dt>
            <dd><a href="https://github.com/frsyuki">Furuhashi Sadayuki</a></dd>
            <dt>Description</dt>
            <dd>
                Prestogres is a gateway server that allows clients
                to use PostgreSQL protocol and thus the
                PostgreSQL ODBC driver to run queries on Presto.
            </dd>
        </dl>
    </div>

    <h3 id="starburst">Starburst</h3>

    <div class="item">
        <h4>Starburst ODBC Driver</h4>
        <dl>
            <dt>Project</dt>
            <dd><a href="https://www.starburstdata.com/our-offerings/#drivers-block">Starburst Enterprise ODBC/JDBC Presto Drivers</a></dd>
            <dt>Maintained by</dt>
            <dd><a href="https://www.starburstdata.com/">Starburst, The Presto company</a></dd>
            <dt>Description</dt>
            <dd>
                The Starburst Enterprise Client Drivers for Presto include
                enterprise grade ODBC and JDBC drivers enabling you to
                use your preferred Business Intelligence tools with Presto.
                The drivers fully implement the ODBC and JDBC specifications
                and are compatible with the
                <a href="https://www.starburstdata.com/our-offerings/">Enterprise Starburst Presto release</a>
                which is available for download.
                There are ODBC drivers for Windows, Mac, and Linux platforms.
                Starburst additionally provides
                <a href="https://www.starburstdata.com/presto-enterprise/">enterprise Presto support and services</a>
            </dd>
        </dl>
    </div>

    <h2 id="libraries">Presto Libraries</h2>

    <p>
        The following client libraries can be used to run queries from
        several programming languages:
        <a href="#language-c">C</a>,
        <a href="#language-go">Go</a>,
        <a href="#language-java">Java</a>,
        <a href="#language-node">Node.js</a>,
        <a href="#language-python">Python</a>,
        <a href="#language-r">R</a>,
        <a href="#language-ruby">Ruby</a>.
    </p>

    <h3 id="language-c">Language: C</h3>

    <div class="item">
        <h4>PrestoClient C</h4>
        <dl>
            <dt>Project</dt>
            <dd><a href="https://github.com/easydatawarehousing/prestoclient/tree/master/C">GitHub</a></dd>
            <dt>Maintained by</dt>
            <dd><a href="https://github.com/easydatawarehousing">Ivo Herweijer</a></dd>
            <dt>Description</dt>
            <dd>C client for Presto.</dd>
        </dl>
    </div>

    <h3 id="language-go">Language: Go</h3>

    <div class="item">
        <h4>presto-go-client</h4>
        <dl>
            <dt>Project</dt>
            <dd><a href="https://github.com/prestodb/presto-go-client">GitHub</a></dd>
            <dt>Maintained by</dt>
            <dd><a href="https://github.com/prestodb/presto-go-client">Presto Go Client Team</a></dd>
            <dt>Description</dt>
            <dd>Go client for Presto.</dd>
        </dl>
    </div>

    <h3 id="language-java">Language: Java</h3>

    <div class="item">
        <h4>Presto JDBC Driver</h4>
        <dl>
            <dt>Project</dt>
            <dd><a href="docs/current/installation/jdbc.html">Presto</a></dd>
            <dt>Maintained by</dt>
            <dd><a href="https://github.com/prestosql/presto">Presto Team</a></dd>
            <dt>Description</dt>
            <dd>JDBC driver for Presto.</dd>
            <dt>Example</dt>
            <dd>
<pre>
String sql = "SELECT * FROM example";
String url = "jdbc:presto://localhost:8080/catalog/schema";
try (Connection connection =
    DriverManager.getConnection(url, "test", null)) {
try (Statement statement = connection.createStatement()) {
    try (ResultSet rs = statement.executeQuery(sql)) {
        while (rs.next()) {
            System.out.println(rs.getString("node_id"));
        }
    }
}
}
</pre>
            </dd>
        </dl>
    </div>

    <h3 id="language-node">Language: Node.js</h3>

    <div class="item">
        <h4>presto-client-node</h4>
        <dl>
            <dt>Project</dt>
            <dd><a href="https://github.com/tagomoris/presto-client-node">GitHub</a></dd>
            <dt>Maintained by</dt>
            <dd><a href="https://github.com/tagomoris">Satoshi Tagomori</a></dd>
            <dt>Description</dt>
            <dd>Node.js client for Presto.</dd>
        </dl>
    </div>

    <h3 id="language-python">Language: Python</h3>

    <div class="item">
        <h4>presto-python-client</h4>
        <dl>
            <dt>Project</dt>
            <dd><a href="https://github.com/prestodb/presto-python-client">GitHub</a></dd>
            <dt>Maintained by</dt>
            <dd><a href="https://github.com/prestodb/presto-python-client">Presto Python Client Team</a></dd>
            <dt>Description</dt>
            <dd>Python client for Presto.</dd>
        </dl>
    </div>

    <div class="item">
        <h4>PyHive</h4>
        <dl>
            <dt>Project</dt>
            <dd><a href="https://github.com/dropbox/PyHive">GitHub</a></dd>
            <dt>Maintained by</dt>
            <dd><a href="https://github.com/dropbox">Dropbox</a></dd>
            <dt>Description</dt>
            <dd>PyHive is a collection of Python DB-API and SQLAlchemy interfaces for Presto and Hive.</dd>
        </dl>
    </div>

    <div class="item">
        <h4>PrestoClient Python</h4>
        <dl>
            <dt>Project</dt>
            <dd><a href="https://github.com/easydatawarehousing/prestoclient/tree/master/python">GitHub</a></dd>
            <dt>Maintained by</dt>
            <dd><a href="https://github.com/easydatawarehousing">Ivo Herweijer</a></dd>
            <dt>Description</dt>
            <dd>Python client for Presto.</dd>
        </dl>
    </div>

    <h3 id="language-r">Language: R</h3>

    <div class="item">
        <h4>RPresto</h4>
        <dl>
            <dt>Project</dt>
            <dd><a href="https://github.com/prestodb/RPresto">GitHub</a></dd>
            <dt>Maintained by</dt>
            <dd><a href="https://github.com/prestodb/RPresto">RPresto Team</a></dd>
            <dt>Description</dt>
            <dd>DBI-based adapter for Presto for R.</dd>
        </dl>
    </div>

    <h3 id="language-ruby">Language: Ruby</h3>

    <div class="item">
        <h4>presto-client-ruby</h4>
        <dl>
            <dt>Project</dt>
            <dd><a href="https://github.com/treasure-data/presto-client-ruby">GitHub</a></dd>
            <dt>Maintained by</dt>
            <dd><a href="https://github.com/frsyuki">Furuhashi Sadayuki</a></dd>
            <dt>Description</dt>
            <dd>Ruby client for Presto.</dd>
        </dl>
    </div>

    <h2 id="guis">Presto GUIs</h2>

    <div class="item">
        <h4>Airpal</h4>
        <dl>
            <dt>Project</dt>
            <dd><a href="https://airbnb.github.io/airpal/">Airpal</a></dd>
            <dt>Maintained by</dt>
            <dd><a href="https://github.com/airbnb">Airbnb</a></dd>
            <dt>Description</dt>
            <dd>
                Airpal is a web-based, query execution tool which
                leverages Presto to make authoring queries
                and retrieving results simple for users. Airpal provides
                the ability to find tables, see metadata, browse sample
                rows, write and edit queries, then submit queries all
                in a web interface.
            </dd>
        </dl>
    </div>

    <div class="item">
        <h4>Redash</h4>
        <dl>
            <dt>Project</dt>
            <dd><a href="https://redash.io/">Redash</a></dd>
            <dt>Maintained by</dt>
            <dd><a href="https://github.com/getredash/">Arik Fraimovich</a></dd>
            <dt>Description</dt>
            <dd>
                Redash is a take on freeing the data within our
                company in a way that will better fit our culture and
                usage patterns. It has Presto support as well as other
                backends, and offers a query editor with syntax
                highlighting and completion, and creating
                visualizations and dashboards from query results.
            </dd>
        </dl>
    </div>

    <div class="item">
        <h4>Shib</h4>
        <dl>
            <dt>Project</dt>
            <dd><a href="https://github.com/tagomoris/shib">GitHub</a></dd>
            <dt>Maintained by</dt>
            <dd><a href="https://github.com/tagomoris">Tagomori Satoshi</a></dd>
            <dt>Description</dt>
            <dd>
                Shib is a web-client written in Node.js designed to
                query Presto and Hive. To run Shib install node.js,
                alter your config.js, and follow the instructions on
                the shib project page. Shib can also be used as an
                proxy server for query engines.
            </dd>
        </dl>
    </div>

    <div class="item">
        <h4>Superset</h4>
        <dl>
            <dt>Project</dt>
            <dd><a href="https://superset.incubator.apache.org/">Apache Superset</a></dd>
            <dt>Maintained by</dt>
            <dd><a href="https://github.com/apache/incubator-superset">Apache Superset</a></dd>
            <dt>Description</dt>
            <dd>
                Superset enables users to consume data in many different
                ways: writing SQL queries, creating new tables, creating
                a visualization (slice), adding that visualization to one
                or many dashboards and downloading a CSV. SQL Lab is a
                a part of Superset and provides rich SQL editor that
                enables users to both query and visualize data.
                You can explore and preview tables in Presto, effortlessly
                compose SQL queries to access data. From there, you can
                either export a CSV file or immediately visualize your
                data in the Superset "Explore" view.
            </dd>
        </dl>
    </div>

    <div class="item">
        <h4>yanagishima</h4>
        <dl>
            <dt>Project</dt>
            <dd><a href="https://github.com/wyukawa/yanagishima">GitHub</a></dd>
            <dt>Maintained by</dt>
            <dd><a href="https://github.com/wyukawa">wyukawa</a>, <a href="https://github.com/okazou">okazou</a></dd>
            <dt>Description</dt>
            <dd>
                yanagishima is a web application for Presto.
                yanagishima provides the ability to execute query,
                show query, kill query, bookmark query, search table,
                share query/query result, format query, download as CSV/TSV file,
                insert chart, substitute query parameter, and so on.
            </dd>
        </dl>
    </div>

    <h2 id="tools">Presto Management Tools</h2>

    <div class="item">
        <h4>Presto-Admin</h4>
        <dl>
            <dt>Project</dt>
            <dd><a href="https://github.com/prestosql/presto-admin">Presto-Admin</a></dd>
            <dt>Maintained by</dt>
            <dd><a href="https://www.starburstdata.com/">Starburst, The Presto company</a></dd>
            <dt>Description</dt>
            <dd>
                Presto-Admin is a tool for installing and managing the Presto
                query engine on a cluster. It provides easy-to-use commands:
                <ul>
                    <li>Install and uninstall Presto across your cluster</li>
                    <li>Configure your Presto cluster</li>
                    <li>Start and stop the Presto servers</li>
                    <li>Gather status and log information from your Presto cluster</li>
                </ul>
                If you need any assistance with your Presto cluster management
                reach out to <a href="https://www.starburstdata.com">Starburst</a>
                for their <a href="https://www.starburstdata.com/presto-enterprise/">Presto enterprise support</a>
                offering and other Presto related services.
            </dd>
            <dt>Examples</dt>
<pre>
presto-admin server start|stop|restart|status
presto-admin server install path-to-presto-rpm
presto-admin connector add connector-name
</pre>
        </dl>
    </div>

    <h2 id="support">Enterprise Support for Presto</h2>

    <div class="item">
        <h4>Starburst Data</h4>
        <dl>
            <dt>Website</dt>
            <dd><a href="https://www.starburstdata.com/">Starburst, The Presto company</a></dd>
            <dt>Scope</dt>
            <dd>Enterprise 24/7 Support, Installation, Configuration, Training,
                Custom Development, Tuning</dd>
            <dt>Description</dt>
            <dd>
              <p>
                At Starburst, our team is a major contributor to the open source Presto project.
                We consist of many of the <b>experts and committers</b> who have been contributing to
                and advancing the Presto product over the last few years. Starburst provides an
                <a href="https://www.starburstdata.com/our-offerings/">enterprise ready Presto distribution</a>
                and <a href="https://www.starburstdata.com/presto-enterprise/">Presto support</a>.
                Starburst's distribution of Presto consists of additional tooling and
                configurations to make it work well in the enterprise. Further, it is
                rigorously tested at scale and patched as needed. And with our wide range
                of services, support, and training we will help you be successful in this
                new world of open source technologies in the enterprise.
              </p>
              <p>
                In addition to implementing Presto internals to make it the most reliable,
                robust, and performant open source distributed query engine, our team at
                Starburst is dedicated to continually improve and add the needed features
                for the enterprise. Our major enterprise focus areas are ease-of-use, security,
                robustness, wide range of integrations, and reliable support SLAs.
              </p>
            </dd>
        </dl>
    </div>

    <h2 id="hosted">Hosted Presto</h2>

    <div class="item">
        <h4>Qubole</h4>
        <dl>
            <dt>Product</dt>
            <dd><a href="https://www.qubole.com/product/architecture/best-of-breed-engines/">Managed Presto Service</a></dd>
            <dt>Description</dt>
            <dd>
                <p>
                Qubole integrates an enhanced and cloud-optimized version of Presto. 
                Qubole’s Presto implementation is an enterprise-ready and secure distributed 
                SQL query engine, which allows analysts to quickly derive business insights from data.
                </p>
                <p>
                Qubole has optimized Presto for the cloud. Qubole’s enhancements allow for 
                dynamic cluster sizing based on workload and termination of idle clusters — ensuring high 
                reliability while reducing compute costs. Qubole’s Presto clusters support multi-tenancy 
                and provide logs and metrics to track performance of queries.
                </p>
            </dd>
        </dl>
    </div>

    <div class="item">
        <h4>Amazon Athena</h4>
        <dl>
            <dt>Website</dt>
            <dd><a href="https://aws.amazon.com/athena/">Amazon Athena</a></dd>
            <dt>Maintainer</dt>
            <dd><a href="https://aws.amazon.com/">Amazon Web Services</a></dd>
            <dd>
                <p>
                    Amazon Athena is an interactive query service based on Presto that makes it easy to analyze data in Amazon S3
                    using standard SQL. Athena is serverless, so there is no infrastructure to manage, and you pay only for the
                    queries that you run.
                </p>
                <p>
                    Amazon Athena uses Presto with full standard SQL support and works with a variety of standard data formats.
                    Athena is out-of-the-box integrated with AWS Glue Data Catalog, allowing you to create a unified metadata
                    repository across various services, crawl data sources to discover schemas and populate your Catalog with
                    new and modified table and partition definitions, and maintain schema versioning.
                </p>
            </dd>
        </dl>
    </div>

    <h2 id="cloud">Presto Cloud</h2>

    <p>
        Presto is also readily available in <a href="#aws">AWS</a> and <a href="#azure">Azure</a> cloud environments.
    </p>

    <h3 id="aws">AWS</h3>

    <div class="item">
        <h4>Starburst Presto</h4>
        <dl>
            <dt>Website</dt>
            <dd><a href="https://www.starburstdata.com/presto-aws-cloud/">Presto on AWS</a></dd>
            <dt>Maintainer</dt>
            <dd><a href="https://www.starburstdata.com/">Starburst, The Presto company</a></dd>
            <dd>
                <p>
                    Starburst Presto on AWS combines the reliable, scalable, and cost-effective
                    cloud computing services provided by Amazon Web Services (AWS) with the power of Presto,
                    the fastest growing distributed SQL query engine within the industry.
                </p>
                <p>
                    Through the use of Starburst’s CloudFormation template and Starburst Presto AMI,
                    Starburst Presto on AWS enables you to run analytic SQL queries across
                    a wide variety of data sources with elastic scaling and usage-based pricing.
                    Read more how to use Presto on AWS on our <a href="https://docs.starburstdata.com/latest/aws.html">AWS Documentation site</a>.
                </p>
            </dd>
        </dl>
    </div>

   <div class="item">
       <h4>Amazon EMR</h4>
       <dl>
           <dt>Website</dt>
           <dd><a href="https://aws.amazon.com/emr/">Amazon EMR</a></dd>
           <dt>Maintainer</dt>
           <dd><a href="https://aws.amazon.com/">Amazon Web Services</a></dd>
           <dd>
               <p>
                   Amazon EMR provides a managed Hadoop framework that makes it easy, fast, and cost-effective
                   to process vast amounts of data across dynamically scalable Amazon EC2 instances. With EMR, you can launch a
                   large Presto cluster in minutes. You don't need to worry about node provisioning, cluster setup or tuning.
               </p>
               <p>
                   Using Presto on EMR provides these benefits to customers:
                   <ul>
                       <li>Elasticity: With Amazon EMR, you can provision one, hundreds, or thousands of compute instances to
                           process data at any scale. You can easily increase or decrease the number of instances manually
                           or with Auto Scaling, and you only pay for what you use.</li>
                       <li>Simple and predictable pricing: You pay a per-second rate for every second used, with a one-minute
                           minimum charge.</li>
                   </ul>
               </p>
           </dd>
       </dl>
   </div>

    <h3 id="azure">Azure</h3>

    <div class="item">
        <h4>Starburst Presto</h4>
        <dl>
            <dt>Website</dt>
            <dd><a href="https://www.starburstdata.com/presto-azure/">Presto on Azure</a></dd>
            <dt>Maintainer</dt>
            <dd><a href="https://www.starburstdata.com/">Starburst, The Presto company</a></dd>
            <dd>
                <p>
                    Starburst Presto for HDInsight is a distributed SQL query engine that is integrated
                    into Azure HDInsight Platform and available via the Azure Marketplace.
                </p>
                <p>
                    Azure HDInsight is a fully-managed cloud service that makes it easy, fast,
                    and cost-effective to process massive amounts of data. Presto and HDInsight were
                    both designed for the separation of storage and compute which allows for flexible
                    performance and cost. You pay only for what you use by creating clusters on demand
                    scaling them up and down.
                    Read more how to use Presto on Azure on our <a href="https://docs.starburstdata.com/latest/azure.html">Azure Documentation site</a>.
                </p>
                <p>
                    Integrating Presto with HDInsight provides Azure users with two new capabilities:
                    <ul>
                        <li>A fast, scalable, interactive SQL interface to data in Azure Blob and Azure Data Lake Storage</li>
                        <li>An easy way to integrate data with HDInsight by leveraging Presto’s vast portfolio of data connectors.</li>
                    </ul>
                </p>
            </dd>
        </dl>
    </div>

</div>

<div class="rightcol">
    <h3>Presto Resources</h3>
    <ul>
        <li><a href="#odbc">ODBC</a></li>
        <li><a href="#libraries">Libraries</a></li>
        <li><a href="#guis">GUIs</a></li>
        <li><a href="#tools">Management Tools</a></li>
        <li><a href="#support">Enterprise Support</a></li>
        <li><a href="#hosted">Hosted Presto</a></li>
        <li><a href="#cloud">Cloud</a></li>
    </ul>
</div>
