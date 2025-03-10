<!--
Copyright 2002-2004 The Apache Software Foundation

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
//-->

# Release Notes - ZooKeeper - Version 3.7.2

## Sub-task

* [ZOOKEEPER-4327](https://issues.apache.org/jira/browse/ZOOKEEPER-4327) - Flaky test: RequestThrottlerTest

## Bug

* [ZOOKEEPER-4026](https://issues.apache.org/jira/browse/ZOOKEEPER-4026) - CREATE2 requests embeded in a MULTI request only get a regular CREATE response
* [ZOOKEEPER-4308](https://issues.apache.org/jira/browse/ZOOKEEPER-4308) - Flaky test: EagerACLFilterTest.testSetDataFail
* [ZOOKEEPER-4460](https://issues.apache.org/jira/browse/ZOOKEEPER-4460) - QuorumPeer overrides Thread.getId with different semantics
* [ZOOKEEPER-4511](https://issues.apache.org/jira/browse/ZOOKEEPER-4511) - Flaky test: FileTxnSnapLogMetricsTest.testFileTxnSnapLogMetrics
* [ZOOKEEPER-4537](https://issues.apache.org/jira/browse/ZOOKEEPER-4537) - Race between SyncThread and CommitProcessor thread
* [ZOOKEEPER-4565](https://issues.apache.org/jira/browse/ZOOKEEPER-4565) - Config watch path get truncated abnormally and fail chroot zookeeper client
* [ZOOKEEPER-4654](https://issues.apache.org/jira/browse/ZOOKEEPER-4654) - Fix C client test compilation error in Util.cc.
* [ZOOKEEPER-4674](https://issues.apache.org/jira/browse/ZOOKEEPER-4674) - C client tests don&#39;t pass on CI
* [ZOOKEEPER-4721](https://issues.apache.org/jira/browse/ZOOKEEPER-4721) - Upgrade OWASP Dependency Check to 8.3.1

## Improvement

* [ZOOKEEPER-4545](https://issues.apache.org/jira/browse/ZOOKEEPER-4545) - Backport auto reloading client key/trust store to 3.7
* [ZOOKEEPER-4551](https://issues.apache.org/jira/browse/ZOOKEEPER-4551) - Do not log spammy stacktrace when a client closes its connection
* [ZOOKEEPER-4602](https://issues.apache.org/jira/browse/ZOOKEEPER-4602) - Upgrade reload4j due to XXE vulnerability
* [ZOOKEEPER-4616](https://issues.apache.org/jira/browse/ZOOKEEPER-4616) - Upgrade docker image for the dev enviroment to resolve CVEs
* [ZOOKEEPER-4657](https://issues.apache.org/jira/browse/ZOOKEEPER-4657) - Publish SBOM artifacts
* [ZOOKEEPER-4659](https://issues.apache.org/jira/browse/ZOOKEEPER-4659) - Upgrade Commons CLI to 1.5.0 due to OWASP failing on 1.4 CVE-2021-37533
* [ZOOKEEPER-4660](https://issues.apache.org/jira/browse/ZOOKEEPER-4660) - Suppress false positive OWASP failure for CVE-2021-37533
* [ZOOKEEPER-4661](https://issues.apache.org/jira/browse/ZOOKEEPER-4661) - Upgrade Jackson Databind to 2.13.4.2 for CVE-2022-42003 CVE-2022-42004
* [ZOOKEEPER-4753](https://issues.apache.org/jira/browse/ZOOKEEPER-4753) - Explicit handling of DIGEST-MD5 vs GSSAPI in quorum auth

## Task

* [ZOOKEEPER-4599](https://issues.apache.org/jira/browse/ZOOKEEPER-4599) - Upgrade Jetty to avoid CVE-2022-2048
* [ZOOKEEPER-4627](https://issues.apache.org/jira/browse/ZOOKEEPER-4627) - High CVE-2022-2048 in jetty-*-9.4.46.v20220331.jar fixed in 9.4.47
* [ZOOKEEPER-4632](https://issues.apache.org/jira/browse/ZOOKEEPER-4632) - Fix NPE from ConnectionMetricsTest.testRevalidateCount
* [ZOOKEEPER-4641](https://issues.apache.org/jira/browse/ZOOKEEPER-4641) - GH CI fails with error: implicit declaration of function FIPS_mode
* [ZOOKEEPER-4649](https://issues.apache.org/jira/browse/ZOOKEEPER-4649) - Upgrade netty to 4.1.86 because of CVE-2022-41915
* [ZOOKEEPER-4669](https://issues.apache.org/jira/browse/ZOOKEEPER-4669) - Upgrade snappy-java to 1.1.9.1 (in order to support M1 macs)
* [ZOOKEEPER-4688](https://issues.apache.org/jira/browse/ZOOKEEPER-4688) - Upgrade `cyclonedx-maven-plugin` to 2.7.6
* [ZOOKEEPER-4707](https://issues.apache.org/jira/browse/ZOOKEEPER-4707) - Update snappy-java to address multiple CVEs
* [ZOOKEEPER-4709](https://issues.apache.org/jira/browse/ZOOKEEPER-4709) - Upgrade Netty to 4.1.94.Final
* [ZOOKEEPER-4716](https://issues.apache.org/jira/browse/ZOOKEEPER-4716) - Upgrade jackson to 2.15.2, suppress two false positive CVE errors
* [ZOOKEEPER-4751](https://issues.apache.org/jira/browse/ZOOKEEPER-4751) - Update snappy-java to 1.1.10.5 to address CVE-2023-43642
* [ZOOKEEPER-4754](https://issues.apache.org/jira/browse/ZOOKEEPER-4754) - Update Jetty to avoid CVE-2023-36479, CVE-2023-40167, and CVE-2023-41900
* [ZOOKEEPER-4755](https://issues.apache.org/jira/browse/ZOOKEEPER-4755) - Handle Netty CVE-2023-4586

&nbsp;


# Release Notes - ZooKeeper - Version 3.7.1

## Improvement

* [ZOOKEEPER-3798](https://issues.apache.org/jira/browse/ZOOKEEPER-3798) - remove the useless code in the ProposalRequestProcessor#processRequest
* [ZOOKEEPER-3807](https://issues.apache.org/jira/browse/ZOOKEEPER-3807) - fix the bad format when website pages build due to bash marker
* [ZOOKEEPER-3841](https://issues.apache.org/jira/browse/ZOOKEEPER-3841) - remove useless codes in the Leader.java
* [ZOOKEEPER-4259](https://issues.apache.org/jira/browse/ZOOKEEPER-4259) - Allow AdminServer to force https
* [ZOOKEEPER-4281](https://issues.apache.org/jira/browse/ZOOKEEPER-4281) - Packet length sanity check is inconsistent
* [ZOOKEEPER-4284](https://issues.apache.org/jira/browse/ZOOKEEPER-4284) - Add metrics for observer sync time
* [ZOOKEEPER-4312](https://issues.apache.org/jira/browse/ZOOKEEPER-4312) - ZooKeeperServerEmbedded: enhance server start/stop for testability
* [ZOOKEEPER-4318](https://issues.apache.org/jira/browse/ZOOKEEPER-4318) - Only report the follower sync time metrics if sync is completed
* [ZOOKEEPER-4355](https://issues.apache.org/jira/browse/ZOOKEEPER-4355) - ZK documentation side bar and welcome page are out of sync
* [ZOOKEEPER-4380](https://issues.apache.org/jira/browse/ZOOKEEPER-4380) - Avoid NPE in RateLogger#rateLimitLog
* [ZOOKEEPER-4382](https://issues.apache.org/jira/browse/ZOOKEEPER-4382) - Update Maven Bundle Plugin in order to allow builds on JDK18
* [ZOOKEEPER-4453](https://issues.apache.org/jira/browse/ZOOKEEPER-4453) - NettyServerCnxnFactory: allow to configure the early TLS connection drop feature
* [ZOOKEEPER-4454](https://issues.apache.org/jira/browse/ZOOKEEPER-4454) - Upgrade Netty to 4.1.73
* [ZOOKEEPER-4455](https://issues.apache.org/jira/browse/ZOOKEEPER-4455) - Move to https://reload4j.qos.ch/ (remove log4j1)
* [ZOOKEEPER-4462](https://issues.apache.org/jira/browse/ZOOKEEPER-4462) - Upgrade Netty TCNative to 2.0.48
* [ZOOKEEPER-4468](https://issues.apache.org/jira/browse/ZOOKEEPER-4468) - Backport BCFKS key/trust store format support to branch 3.5
* [ZOOKEEPER-4529](https://issues.apache.org/jira/browse/ZOOKEEPER-4529) - Upgrade netty to 4.1.76.Final
* [ZOOKEEPER-4531](https://issues.apache.org/jira/browse/ZOOKEEPER-4531) - Revert Netty TCNative change

## Bug

* [ZOOKEEPER-1875](https://issues.apache.org/jira/browse/ZOOKEEPER-1875) - NullPointerException in ClientCnxn$EventThread.processEvent
* [ZOOKEEPER-3128](https://issues.apache.org/jira/browse/ZOOKEEPER-3128) - Get CLI Command displays Authentication error for Authorization error
* [ZOOKEEPER-3652](https://issues.apache.org/jira/browse/ZOOKEEPER-3652) - Improper synchronization in ClientCnxn
* [ZOOKEEPER-3887](https://issues.apache.org/jira/browse/ZOOKEEPER-3887) - In SSL-only server zkServer.sh status command should use secureClientPortAddress instead of clientPortAddress
* [ZOOKEEPER-3988](https://issues.apache.org/jira/browse/ZOOKEEPER-3988) - org.apache.zookeeper.server.NettyServerCnxn.receiveMessage throws NullPointerException
* [ZOOKEEPER-4194](https://issues.apache.org/jira/browse/ZOOKEEPER-4194) - ZooInspector throws NullPointerExceptions to console when node data is null
* [ZOOKEEPER-4204](https://issues.apache.org/jira/browse/ZOOKEEPER-4204) - Flaky test - RequestPathMetricsCollectorTest.testMultiThreadPerf
* [ZOOKEEPER-4247](https://issues.apache.org/jira/browse/ZOOKEEPER-4247) - NPE while processing message from restarted quorum member
* [ZOOKEEPER-4265](https://issues.apache.org/jira/browse/ZOOKEEPER-4265) - Download page broken links
* [ZOOKEEPER-4266](https://issues.apache.org/jira/browse/ZOOKEEPER-4266) - Correct ZooKeeper version in documentation header
* [ZOOKEEPER-4269](https://issues.apache.org/jira/browse/ZOOKEEPER-4269) - acceptedEpoch.tmp rename failure will cause server startup error
* [ZOOKEEPER-4272](https://issues.apache.org/jira/browse/ZOOKEEPER-4272) - Upgrade Netty library to > 4.1.60 due to security vulnerability CVE-2021-21295
* [ZOOKEEPER-4275](https://issues.apache.org/jira/browse/ZOOKEEPER-4275) - Slowness in sasl login or subject.doAs() causes zk client to falsely assume that the server did not respond, closes connection and goes to unnecessary retries
* [ZOOKEEPER-4277](https://issues.apache.org/jira/browse/ZOOKEEPER-4277) - dependency-check:check failing - jetty-server-9.4.38 CVE-2021-28165
* [ZOOKEEPER-4278](https://issues.apache.org/jira/browse/ZOOKEEPER-4278) - dependency-check:check failing - netty-transport-4.1.60.Final CVE-2021-21409
* [ZOOKEEPER-4309](https://issues.apache.org/jira/browse/ZOOKEEPER-4309) - QuorumCnxManager's ListenerHandler thread leak
* [ZOOKEEPER-4331](https://issues.apache.org/jira/browse/ZOOKEEPER-4331) - zookeeper artifact is not compatible with OSGi runtime
* [ZOOKEEPER-4337](https://issues.apache.org/jira/browse/ZOOKEEPER-4337) - CVE-2021-34429 in jetty 9.4.38.v20210224 in zookeeper 3.7.0
* [ZOOKEEPER-4342](https://issues.apache.org/jira/browse/ZOOKEEPER-4342) - Robustify C client against errors during SASL negotiation
* [ZOOKEEPER-4345](https://issues.apache.org/jira/browse/ZOOKEEPER-4345) - Avoid NoSunchMethodException caused by shaded zookeeper jar
* [ZOOKEEPER-4356](https://issues.apache.org/jira/browse/ZOOKEEPER-4356) - Code blocks do not render correctly in ZK docs site
* [ZOOKEEPER-4360](https://issues.apache.org/jira/browse/ZOOKEEPER-4360) - Avoid NPE during metrics execution if the leader is not set on a FOLLOWER node
* [ZOOKEEPER-4362](https://issues.apache.org/jira/browse/ZOOKEEPER-4362) - ZKDatabase.txnCount logged non transactional requests
* [ZOOKEEPER-4367](https://issues.apache.org/jira/browse/ZOOKEEPER-4367) - Zookeeper#Login thread leak in case of Sasl AuthFailed.
* [ZOOKEEPER-4377](https://issues.apache.org/jira/browse/ZOOKEEPER-4377) - KeeperException.create has NullPointerException when low version client requests the high version server
* [ZOOKEEPER-4452](https://issues.apache.org/jira/browse/ZOOKEEPER-4452) - Log4j 1.X CVE-2022-23302/5/7 vulnerabilities
* [ZOOKEEPER-4477](https://issues.apache.org/jira/browse/ZOOKEEPER-4477) - Single Kerberos ticket renewal failure can prevent all future renewals since Java 9
* [ZOOKEEPER-4504](https://issues.apache.org/jira/browse/ZOOKEEPER-4504) - ZKUtil#deleteRecursive causing deadlock in HDFS HA functionality
* [ZOOKEEPER-4505](https://issues.apache.org/jira/browse/ZOOKEEPER-4505) - CVE-2020-36518 - Upgrade jackson databind to 2.13.2.1
* [ZOOKEEPER-4510](https://issues.apache.org/jira/browse/ZOOKEEPER-4510) - dependency-check:check failing - reload4j-1.2.19.jar: CVE-2020-9493, CVE-2022-23307
* [ZOOKEEPER-4514](https://issues.apache.org/jira/browse/ZOOKEEPER-4514) - ClientCnxnSocketNetty throwing NPE
* [ZOOKEEPER-4515](https://issues.apache.org/jira/browse/ZOOKEEPER-4515) - ZK Cli quit command always logs error
* [ZOOKEEPER-4516](https://issues.apache.org/jira/browse/ZOOKEEPER-4516) - checkstyle:check is failing

## Test

* [ZOOKEEPER-4333](https://issues.apache.org/jira/browse/ZOOKEEPER-4333) - QuorumSSLTest - testOCSP fails on JDK17

## Task

* [ZOOKEEPER-3970](https://issues.apache.org/jira/browse/ZOOKEEPER-3970) - Enable ZooKeeperServerController to expire session
* [ZOOKEEPER-4315](https://issues.apache.org/jira/browse/ZOOKEEPER-4315) - Fix NOTICE file in the source distribution
* [ZOOKEEPER-4414](https://issues.apache.org/jira/browse/ZOOKEEPER-4414) - Update Netty to 4.1.70.Final
* [ZOOKEEPER-4429](https://issues.apache.org/jira/browse/ZOOKEEPER-4429) - Update jackson-databind to 2.13.1
* [ZOOKEEPER-4469](https://issues.apache.org/jira/browse/ZOOKEEPER-4469) - Suppress OWASP false positives related to Netty TCNative
* [ZOOKEEPER-4478](https://issues.apache.org/jira/browse/ZOOKEEPER-4478) - Suppress OWASP false positives zookeeper-jute-3.8.0-SNAPSHOT.jar: CVE-2021-29425, CVE-2021-28164, CVE-2021-34429
* [ZOOKEEPER-4479](https://issues.apache.org/jira/browse/ZOOKEEPER-4479) - Tests: C client test TestOperations.cc testTimeoutCausedByWatches1 is very flaky on CI
* [ZOOKEEPER-4482](https://issues.apache.org/jira/browse/ZOOKEEPER-4482) - Fix LICENSE FILES for commons-io and commons-cli

## Sub-task

* [ZOOKEEPER-3774](https://issues.apache.org/jira/browse/ZOOKEEPER-3774) - Close quorum socket asynchronously on the leader to avoid ping being blocked by long socket closing time
* [ZOOKEEPER-4251](https://issues.apache.org/jira/browse/ZOOKEEPER-4251) - Flaky test: org.apache.zookeeper.test.WatcherTest
* [ZOOKEEPER-4257](https://issues.apache.org/jira/browse/ZOOKEEPER-4257) - learner.asyncSending, learner.closeSocketAsync and leader.closeSocketAsync should be configurable in zoo.cfg
* [ZOOKEEPER-4270](https://issues.apache.org/jira/browse/ZOOKEEPER-4270) - Flaky test: QuorumPeerMainTest#testLeaderOutOfView
