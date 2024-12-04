To ensure that your tests don't interfere with your production database, you can easily switch to a testing database for PHPUnit. Here's a step-by-step guide:

### Step 1: Create a Testing Database

Copy and paste your `database.sqlite` file and rename it to `testing.sqlite` (or any other name you prefer).

### Step 2: Open `phpunit.xml`

Locate and open the `phpunit.xml` file in your project.

### Step 3: Configure Environment Variable

Add the following environment variable to `phpunit.xml`:

```xml
<env name="DB_DATABASE" value="database/testing.sqlite"/>
```

This tells PHPUnit to use the `testing.sqlite` database for testing purposes.

### Step 4: Run Your Tests

Run your tests as you normally would. From now on, PHPUnit will use the `testing.sqlite` database, leaving your production database intact.

By following these simple steps, you can ensure that your tests don't interfere with your production database, and you can test your application with confidence!
