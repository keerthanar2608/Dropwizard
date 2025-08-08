# Dropwizard


## Step 1: build.gradle.kts:
  Import all required dependencies
  Add Application in Plugin
  Create Application with mainClass.set("ApplicationKt")


## Step 2: src/main/kotlin:
    -`src/main/kotlin/Attendance.kt`
          This file should contain data class which consists of employeeId , CheckIn , CheckOut
    -`src/main/kotlin\AttendanceManager.kt`:
          This files creates mutableList of type Attendance to store all details
    -`src/main/kotlin/AttendanceResource.kt`:
          The AttendanceResource file contains all resource classes like @GET , @POST , @PATH etc..
          @POST will add the details to mutableList
          @GET will return all stored records
    -`src/main/kotlin/AttendanceServiceConfig.kt`:
          This is the Configuration file
    -`src/main/kotlin/AttendanceServiceApp.kt`:
          This AttendanceServiceApp is the Application file which is of type AttendanceConfiguration

## Step 3 : src/main/kotlin/resources:
    -`src/main/kotlin/resources/config.yml`:
           This config file will contain :
                       type 
                       port

