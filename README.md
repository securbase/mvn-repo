# Como integrar este 'repo' de maven temporal

```xml
<repositories>
  <repository>
    <id>mvn-repo</id>
    <url>https://raw.githubusercontent.com/securbase/mvn-repo/master</url>
    <releases>
      <enabled>true</enabled>
    </releases>
    <snapshots>
      <enabled>true</enabled>
    </snapshots>
  </repository>
</repositories>

<properties>
  <sobio-api-client.version>20220801.2d456c4</sobio-api-client.version>
</properties>

<dependencies>
  <dependency>
    <groupId>ar.com.sdc.sobio</groupId>
    <artifactId>sobio-api-client</artifactId>
    <version>${sobio-api-client.version}</version>
  </dependency>

  ...

  <dependency>
    <groupId>com.securbase.biomix.blacklist</groupId>
    <artifactId>biomix-blacklist-api-client</artifactId>
    <version>20240925.2820f8c</version>
  </dependency>

  ...

  <dependency>
    <groupId>com.securbase.biomix_animal.client</groupId>
    <artifactId>biomix_animal_api</artifactId>
    <version>20250325-150849_0.1.0</version>
  </dependency>

</dependencies>

```
