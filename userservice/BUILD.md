# Building and Running the User Service

## Issue with Code Runner

The Code Runner extension compiles Java files directly without resolving Maven dependencies. Spring Boot projects require Maven to manage dependencies.

## Solutions

### Option 1: Use Java Extension Pack (Recommended)

1. Install the "Extension Pack for Java" in VS Code/Cursor
2. This will automatically handle Maven dependencies and Spring Boot
3. Use `F5` to run/debug, or use the Java extension's built-in run commands

### Option 2: Use Maven Commands

If you have Maven installed, use these commands:

**Build the project:**

```bash
mvn clean compile
```

**Run the application:**

```bash
mvn spring-boot:run
```

**Package the application:**

```bash
mvn clean package
```

### Option 3: Install Maven

If Maven is not installed:

1. Download from: https://maven.apache.org/download.cgi
2. Add Maven to your system PATH
3. Verify installation: `mvn --version`
