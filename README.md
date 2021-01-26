# microservice
<?xml version="1.0" encoding="UTF-8"?>
<project xmlns="http://maven.apache.org/POM/4.0.0"
	xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
	xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 https://maven.apache.org/xsd/maven-4.0.0.xsd">
	<modelVersion>4.0.0</modelVersion>
	<parent>
		<groupId>org.springframework.boot</groupId>
		<artifactId>spring-boot-starter-parent</artifactId>
		<version>2.4.2</version>
		<relativePath /> <!-- lookup parent from repository -->
	</parent>
	<groupId>com.adamzareba.spring.security</groupId>
	<artifactId>oauth2</artifactId>
	<version>0.0.1-SNAPSHOT</version>
	<name>oauth2</name>
	<description>Demo project for Spring Boot</description>
	<properties>
		<java.version>1.8</java.version>
		<h2.version>1.4.196</h2.version>
		<postgresql.version>42.1.4</postgresql.version>

		<spring.version>5.0.2.RELEASE</spring.version>
		<spring.hateoas.version>0.24.0.RELEASE</spring.hateoas.version>

		<hibernate.version>5.2.12.Final</hibernate.version>
		<flywaydb.version>5.0.5</flywaydb.version>
		<jackson.version>2.9.5</jackson.version>
		<lombok.version>1.16.20</lombok.version>
		<oauth2.version>2.2.1.RELEASE</oauth2.version>
	</properties>


	<dependencies>
		<!-- <dependency> <groupId>org.springframework.boot</groupId> <artifactId>spring-boot-starter-oauth2-client</artifactId> 
			</dependency> <dependency> <groupId>org.springframework.boot</groupId> <artifactId>spring-boot-starter-oauth2-resource-server</artifactId> 
			</dependency> -->

		<dependency>
			<groupId>org.springframework.boot</groupId>
			<artifactId>spring-boot-starter-test</artifactId>
			<scope>test</scope>
		</dependency>

		<dependency>
			<groupId>org.springframework.boot</groupId>
			<artifactId>spring-boot-starter-web</artifactId>
		</dependency>
		<dependency>
			<groupId>org.springframework.boot</groupId>
			<artifactId>spring-boot-starter-data-jpa</artifactId>
		</dependency>
		<dependency>
			<groupId>org.springframework.boot</groupId>
			<artifactId>spring-boot-starter-security</artifactId>
		</dependency>

		<dependency>
			<groupId>org.springframework</groupId>
			<artifactId>spring-context-support</artifactId>
			<version>${spring.version}</version>
		</dependency>
		<!-- https://mvnrepository.com/artifact/org.springframework.hateoas/spring-hateoas -->
		<dependency>
			<groupId>org.springframework.hateoas</groupId>
			<artifactId>spring-hateoas</artifactId>
			<version>1.0.2.RELEASE</version>
		</dependency>


		<dependency>
			<groupId>com.h2database</groupId>
			<artifactId>h2</artifactId>
			<version>${h2.version}</version>
		</dependency>
		<dependency>
			<groupId>org.postgresql</groupId>
			<artifactId>postgresql</artifactId>
			<version>${postgresql.version}</version>
		</dependency>

		<dependency>
			<groupId>org.hibernate</groupId>
			<artifactId>hibernate-jpamodelgen</artifactId>
			<version>${hibernate.version}</version>
		</dependency>
		<dependency>
			<groupId>org.flywaydb</groupId>
			<artifactId>flyway-core</artifactId>
			<version>5.2.3</version>
		</dependency>
		<dependency>
			<groupId>com.fasterxml.jackson.core</groupId>
			<artifactId>jackson-databind</artifactId>
			<version>2.10.5</version>
		</dependency>
		<!-- https://mvnrepository.com/artifact/com.fasterxml.jackson.datatype/jackson-datatype-hibernate5 -->
		<dependency>
			<groupId>com.fasterxml.jackson.datatype</groupId>
			<artifactId>jackson-datatype-hibernate5</artifactId>
			<version>2.10.5</version>
		</dependency>
		<dependency>
			<groupId>org.projectlombok</groupId>
			<artifactId>lombok</artifactId>
			<version>${lombok.version}</version>
		</dependency>

		<dependency>
			<groupId>org.springframework.security.oauth</groupId>
			<artifactId>spring-security-oauth2</artifactId>
			<version>${oauth2.version}</version>
		</dependency>

	</dependencies>

	<build>
		<plugins>
			<plugin>
				<groupId>org.springframework.boot</groupId>
				<artifactId>spring-boot-maven-plugin</artifactId>
			</plugin>
		</plugins>
	</build>

</project>
