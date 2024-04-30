---
title: Aspose.Imaging Improves Performance with Customizable Cache
type: docs
weight: 30
url: /python-net/aspose-imaging-improves-performance-with-customizable-cache/
---

## **Improves Performance with Customizable Cache**
Aspose.Images uses caching for temporary data storage. The mechanism is simple to use, customizable and transparent. It ensures that there are no performance issues during image processing. This article explains how to customize the cache with Aspose.Imaging API for Python via .NET.

### **Customizing the Cache**
When a process needs temporary data storage, this storage is allocated in the cache. The cache can be space in memory or on disk and is set by the user. When the temporary data is no longer needed, the space is released. The statistics of the allocated space can be inspected at any time. How Aspose.Imaging allocates and uses caches can be customized. This section describes the various settings and their defaults and the code snippets below show how they can be used.

### **Setting where the Cache is Allocated**
To customize how cache space is allocated, set the CacheType property. By default, the cache is allocated in memory and when there is no more space available in memory, it is allocated to disk. This behavior is captured by Auto mode. Auto mode is is flexible and maximizes performance. There are also other modes:

- CACHE_ON_DISK_ONLY mode: allocation to disk only.
- CACHE_IN_MEMORY_ONLY mode: allocation to memory only.

Selecting CacheOnDiskOnly mode may result in poor performance.

### **Setting the Size of the Cache**
Set the maximum space (in bytes) that can be allocated on disk or memory by setting the set_max_disk_space_for_cache and set_max_memory_for_cache properties respectively. By default, both values are set to 0, meaning that there's no upper limit.

### **Controlling Cache Reallocation**
If there isn't enough space available in memory (as specified by the set_max_memory_for_cache property) when a new cache is allocated, the cache is allocated to disk. If there's not enough space on disk, an exception is thrown. The cache allocation process moves from memory to disk but not vice versa. The property exact_reallocate_only is used to control memory re-allocation. Re-allocation is most likely to occur for pre-allocated caches. It can happen when the system figures out that the allocated space will not be sufficient. If exact_reallocate_only is set to the default value, False, the space is re-allocated to the same medium. When set to True, re-allocation cannot exceed the maximum specified space. In this case the existing allocated in-memory cache (which requires re-allocation) is freed and extended space is allocated on disk.

### **Program Samples**
{{< gist "aspose-com-gists" "738ae5f8f8c529196747b94e49abe952" "control-cache-reallocation.py" >}}
