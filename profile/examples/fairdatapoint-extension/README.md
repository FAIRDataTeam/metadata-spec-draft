# FAIR Data Point custom resources profile extension

Given a FAIR Data Point with custom resource definitions, the resources need a way to indicate their validation artifacts, while also indicating their conformance to the "main" profile. The solution is to create a hierarchy of profiles. Pointing to the main profile using `prof:isProfileOf`, validators can resolve any validation artifacts they encounter and apply them.

:construction: This requires the FAIR Data Point to expose a `prof:Profile`, and have it point to the shapes artifact.
