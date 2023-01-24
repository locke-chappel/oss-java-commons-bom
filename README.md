OSS Commons Bill of Materials
==
This BOM artifact defines the current version of all OSS Commons projects so that dowstream projects can track a single artifact making upgrades easier.

The intended use case is for a parent POM to declare this BOM as a dependency under it's dependency management section so that the end project can simply declare which group/artifact is needed without having to pull in everything in the BOM.

```
<dependencyManagement>
  <dependencies>
    <dependency>
      <groupId>com.github.locke-chappel.oss.commons</groupId>
      <artifactId>bom</artifactId>
      <version>${com.github.lc.oss.common.bom.version}</version>
      <type>pom</type>
      <scope>import</scope>
    </dependency>
  </dependencies>
</dependencyManagement>
```