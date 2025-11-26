# Spring Boot Lab

## 專案簡介

這是一個 Spring Boot 示範專案，展示了如何使用 Spring Boot 建立一個簡單的 RESTful Web 服務。專案包含一個基本的 Hello Controller，提供 `/hello` 端點返回問候訊息。

## 環境需求

- **Java**: 21 或以上版本
- **Maven**: 3.6 或以上版本
- **Spring Boot**: 3.2.7

## 如何執行

1. 克隆專案到本地：
   ```bash
   git clone https://github.com/John0728a/springboot-lab.git
   cd springboot-lab
   ```

2. 使用 Maven 編譯並執行專案：
   ```bash
   ./mvnw spring-boot:run
   ```
   或者在 Windows 上：
   ```bash
   mvnw.cmd spring-boot:run
   ```

3. 應用程式啟動後，可透過以下網址存取：
   ```
   http://localhost:8081/hello
   ```

## 如何執行單元測試

使用 Maven 執行所有單元測試：
```bash
./mvnw test
```
或者在 Windows 上：
```bash
mvnw.cmd test
```

## 專案結構

```
springboot-lab/
├── pom.xml                                          # Maven 專案設定檔
├── src/
│   ├── main/
│   │   ├── java/
│   │   │   └── com/example/springbootlab/
│   │   │       ├── SpringbootLabApplication.java    # 應用程式入口點
│   │   │       └── controller/
│   │   │           └── HelloController.java         # REST 控制器
│   │   └── resources/
│   │       └── application.properties               # 應用程式設定檔
│   └── test/
│       └── java/
│           └── com/example/springbootlab/
│               └── controller/
│                   └── HelloControllerTest.java     # 控制器單元測試
└── README.md                                        # 專案說明文件
```

## 使用到的技術

| 技術 | 說明 |
|------|------|
| **Spring Boot 3.2.7** | 用於快速建立獨立的、生產級別的 Spring 應用程式 |
| **Spring Web** | 提供 RESTful Web 服務支援 |
| **Spring Boot Test** | 提供測試框架支援，包含 JUnit 5 和 MockMvc |
| **Maven** | 專案建構和依賴管理工具 |
| **Java 21** | 程式語言版本 |
