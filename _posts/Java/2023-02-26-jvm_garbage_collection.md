---
layout: post
title: JVM review
cover-img: /assets/img/path.jpg
thumbnail-img: /assets/img/thumb.png
share-img: /assets/img/path.jpg
tags: [jvm]
---



### How to tell if an object is alive?

1. Reference counting.  

   * Consider an object to be alive as long as the number of references to that object is greater than zero.

   * Can not **reclaim** cyclic reference.

2. Reachability analysis
   * Traverse the object graph recursively from **GC roots**.
   * GC roots:
     * Live Thread. 
     * Static variables.
     * Local variables
     * Objects in JNI (Java native interface) native method stack.
     * Objects used as monitors for synchronization 



### 

