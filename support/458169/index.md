---
layout: page
title: "UxStyle support article: UxStyle is blocked from installation on Windows 8.1"
description: ""
---
{% include JB/setup %}

# UxStyle Support

### UxStyle is blocked from installation on Windows 8.1
Last updated: September 9, 2013

### Symptom

When launching the installation package for UxStyle software, you may receive an error similar to the following:

![This program has compatibility issues](/assets/images/458169_1.png)

### Cause

As a result of a compatibility issue with Windows 8.1, and some unfortunate politics, Microsoft has pushed out an
application compatibility "hardblock". Hardblocks are typically applied to an application if the application causes a
catastrophic failure (data loss, blue screen, upgrade process failure, system instability, etc.) or gives users too
much control over the appearance of Windows on their PC.

### Resolution

To resolve this problem, ensure you are using the latest version of UxStyle. Visit [http://uxstyle.com](http://uxstyle.com)
for up-to-date software and support information.

### More Information

Two issues were identified:

1. The UxStyle kernel driver component assumed Windows theme signature code resided in a single page, resulting in a
PROCESS_HAS_LOCKED_PAGES bugcheck if code crossed a page boundary.

2. The UxStyle dynamic disassembler component wrote an incorrect set of machine instructions to memory, resulting
in Windows Shell failures.

### Properties

Ref ID: 458169

Applies to: UxStyle 0.2.2.0 and earlier
