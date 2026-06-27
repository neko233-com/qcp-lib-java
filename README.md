# qcp-lib-java

Java binding for QCP protocol.

## Installation

### Maven

```xml
<dependency>
    <groupId>com.neko233</groupId>
    <artifactId>qcp-lib-java</artifactId>
    <version>1.0.0</version>
</dependency>
```

### Gradle

```groovy
implementation 'com.neko233:qcp-lib-java:1.0.0'
```

## Usage

```java
import com.neko233.qcp.QcpClient;

public class Main {
    public static void main(String[] args) {
        // Create QCP client
        QcpClient client = new QcpClient();
        
        // Connect to server
        client.connect("127.0.0.1", 9000);
        
        // Send data
        client.send("hello".getBytes());
        
        // Receive data
        byte[] buffer = new byte[1024];
        int n = client.receive(buffer);
        
        // Close
        client.close();
    }
}
```

## Features

- Thread-safe
- Non-blocking I/O
- Configurable parameters
- Android compatible

## License

MIT License
