# EnumConverter

A library for converting string value to enum

### Problem solved by the library

When working with tg bots, sometimes you have to convert
string values received in the button callback into enum values.


This library allows you to simplify this process.

## How to use

### Managing conversion

#### @Convertee annotation on class
Annotation say library, that marked class is enum, that must fill by library

Properties:
1. converterBeanName - a bean with this name will be registered by the library for use in business
components to convert string values to enum and back.

#### @ConverteeField annotation on field, owner class must be marked @Convertee
Marked method, that must be called first, when handling command or cb is executed

Properties:
1. stringView - string view of enum value. This value must be passed
to be converted to the enum value. The enum value appears will be converted to this string value.


## P.S.
Library is required Java 17, Lombok 1.18.24 in classpath and plugins
'org.springframework.boot:spring-boot-gradle-plugin:3.1.1','io.spring.gradle:dependency-management-plugin:1.1.1'

If you have any questions or issues - contact me in tg - @Sheduled

##### Sorry for gramma errors, English is not my first language:)
