---
icon: code
---

# DEVELOPERS

{% tabs %}
{% tab title="Gradle" %}
{% hint style="danger" %}
The plugin supports addons compiled with **`Java 17`** or higher, provided that the server is running on a Java version not lower than the one used to compile the addon.
{% endhint %}

```css
repositories {
    maven {
        url "http://api.jetby.org/"
        name "JetbyMC"
    }
}

dependencies {
    compileOnly "org.jetby:libb:api:VERSION"
}
```
{% endtab %}

{% tab title="Maven" %}
{% hint style="danger" %}
The plugin supports addons compiled with <mark style="background-color:red;">**`Java 17`**</mark> or higher, provided that the server is running on a Java version not lower than the one used to compile the addon.
{% endhint %}

```xml
<repository>
  <id>JetbyMC</id>
  <url>http://api.jetby.org/</url>
</repository>

<dependency>
  <groupId>org.jetby.libb</groupId>
  <artifactId>api</artifactId>
  <version>VERSION</version>
  <scope>provided</scope>
</dependency>
```
{% endtab %}
{% endtabs %}
