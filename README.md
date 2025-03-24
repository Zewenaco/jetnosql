
# JetNoSQL 🚀

JetNoSQL is a framework-agnostic Java library that enhances integration with non-relational databases (e.g., MongoDB, Cassandra, DynamoDB, Couchbase) with useful utilities, testing support, and better development speed. Designed to work with Spring Boot, Quarkus, Micronaut, or standalone Java.

---

## 📊 Icons Legend
We use the following icons to indicate the development status of each feature:

- 📝 **Planned**: Feature that has been planned and is awaiting development.  
- 🛠️ **In Progress**: Feature currently under development.  
- ✅ **Implemented**: Feature that is fully developed and tested.  
- 🔍 **Under Evaluation**: Feature being discussed or evaluated for inclusion.  

---

## 💡 Features

### Core Utilities
- 📝 **Framework-agnostic utility functions** - Provide common non-relational database utilities.  
- 🔍 **Transaction Management** - Evaluate the feasibility and usefulness for various databases.  
- 📝 **Database Change Management** - Evaluate the feasibility and usefulness for various databases.  

### Testing Support
- 📝 **Annotation-based Data Injection** - Simplify data loading for integration tests.  
- 📝 **Flexible Test Data Handling** - Load data from JSON, YAML, or custom formats.  

### Database Integrations
#### MongoDB
- 📝 **Enhanced Repository Extensions** - Provide helper methods for advanced MongoDB operations.  
- 📝 **Transaction Utilities** - Facilitate multi-document transactions when supported.  

#### Cassandra
- 📝 **Cassandra Repository Extensions** - Custom queries and advanced data handling.  
- 📝 **Test Utilities** - Mocking and data injection for Cassandra-based tests.  

#### DynamoDB
- 📝 **DynamoDB Repository Extensions** - Utility methods for CRUD and transactional operations.  
- 📝 **Enhanced Query Support** - Simplified APIs for querying and batch operations.  

#### Couchbase
- 📝 **Repository Extensions** - Advanced N1QL support and query optimization.  
- 📝 **Transaction Utilities** - Implement support for Couchbase's transaction features.  

### Framework Integrations
#### Spring Boot
- 📝 **Auto-configuration** - Seamless integration with Spring Boot's configuration.  
- 📝 **Custom Beans** - Provide transactional and data utility beans.  

#### Quarkus
- 📝 **Extension Support** - Quarkus-specific integration for non-relational database utilities.  

#### Micronaut
- 📝 **Bean Support** - Auto-configure beans and utilities.  

---

## 📦 Installation

### Core (Framework-Agnostic)
```kotlin
dependencies {
    implementation("com.github.jetnosql:core:1.0.0")
}
```

### MongoDB Module
```kotlin
dependencies {
    implementation("com.github.jetnosql:mongodb:planned")
}
```

### Cassandra Module
```kotlin
dependencies {
    implementation("com.github.jetnosql:cassandra:planned")
}
```

### DynamoDB Module
```kotlin
dependencies {
    implementation("com.github.jetnosql:dynamodb:planned")
}
```

### Couchbase Module
```kotlin
dependencies {
    implementation("com.github.jetnosql:couchbase:planned")
}
```

### Spring Boot Module
```kotlin
dependencies {
    implementation("com.github.jetnosql:spring-boot:planned")
}
```

### Quarkus Module
```kotlin
dependencies {
    implementation("com.github.jetnosql:quarkus:planned")
}
```

### Micronaut Module
```kotlin
dependencies {
    implementation("com.github.jetnosql:micronaut:planned")
}
```

---

## 🏗️ Architecture

The library follows a modular architecture to maximize flexibility and reusability. Each module is designed to encapsulate specific functionalities without tightly coupling to any framework or database technology.

### 📂 Repository Structure
The project is structured into separate modules for each database and framework, keeping the core logic isolated from integrations.

```
jetnosql/
├── core/               # Framework-independent logic
├── adapters/           # Database-specific implementations
│   ├── mongodb/        # MongoDB-specific utilities
│   ├── cassandra/      # Cassandra-specific utilities
│   ├── dynamodb/       # DynamoDB-specific utilities
│   └── couchbase/      # Couchbase-specific utilities
├── integrations/       # Framework-specific integrations
│   ├── spring-boot/    # Spring Boot support
│   ├── quarkus/        # Quarkus support
│   └── micronaut/      # Micronaut support
└── examples/           # Example projects and demos
```

---

## 💡 Contributing
Contributions are welcome! Please open an issue or submit a pull request with your improvements.

---

## 📜 License
Apache 2.0 License.
