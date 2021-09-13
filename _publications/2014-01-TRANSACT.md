---
title: "Verifying Programs Under Snapshot Isolation and Similar Relaxed Consistency Models"
collection: publications
permalink: /publication/2014-01-transact
excerpt: 
date: 2014-05-01
venue: 'ACM SIGPLAN Workshop on Transactional Computing (TRANSACT)'
paperurl: ''
citation: 'Ismail Kuru, Burcu Kulahcioglu Ozkan, Suha Mutluergil, Serdar Tasiran, Tayfun Elmas and Ernie Cohen. &quot;Verifying Programs Under Snapshot Isolation and Similar Relaxed Consistency Models.&quot; <i>Proceedings of 9<sup>th</sup> ACM SIGPLAN Workshop on Transactional Computing (TRANSACT)</i>, 2014.'
--- 

This paper presents a source-to-source translation technique for encoding SI semantics to C programs so that they can be verified using existing static verification tools like VCC.

[pdf](http://suhaorhun.github.io/files/transact14.pdf)

**Abstract.** We present a static verification approach for programs running under snapshot isolation (SI) and similar relaxed transactional semantics. Relaxed conflict detection schemes such as snapshot isolation (SI) are used widely. Under SI, transactions are no longer guaranteed to be serializable, and the simplicity of reasoning sequentially within a transaction is lost. In this paper, we present an approach for statically verifying properties of transactional programs operating under SI. Differently from earlier work, we handletransactional programs even when they are designed not to beserializable.

We present a source-to-source transformation which augments theprogram with an encoding of the SI semantics. Verifying the resulting program with transformed user annotations and specifications isequivalent to verifying the original transactional program running under SI, a fact we prove formally. Our encoding preserves the modularity and scalability of VCC's verification approach. We applied our method successfully to benchmark programs from the transactional memory literature.