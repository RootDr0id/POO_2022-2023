# Inventory Management System

A Java desktop application for managing inventory, purchases, sales, customers, suppliers, and stock activity. The user interface is built with JavaFX and FXML, while Excel workbooks are used for data storage.

## Features

- **Dashboard** — overview of the application.
- **Inventory management** — view and manage products and stock quantities.
- **Purchases** — record stock purchases and manage supplier information.
- **Sales** — process sales and update stock quantities.
- **Customers and suppliers** — manage contact and business information.
- **Activity journal** — review recorded stock movements.

## Technology Stack

- Java 11
- JavaFX 19 and FXML
- Maven
- MaterialFX
- Ikonli
- Excel workbooks (`.xlsx`) for data storage

## Requirements

- Java 11 or later
- Maven (only required when building the project)

Check your installations:

```bash
java -version
mvn -version
```

## Run the Existing JAR

A packaged application is included in the repository.

From the repository root, run:

```bash
java -jar shade/Main_Project.jar
```

Keep the four Excel workbooks in the repository root when launching the application this way. They are used by the application to read and save data.

## Build from Source

From the repository root, run:

```bash
mvn clean compile package
```

Maven compiles the project and creates the packaged JAR in the `shade/` directory. The build also copies the required Excel workbooks to the appropriate locations.

## Demo Account

| Field | Value |
|---|---|
| Username | `bachir` |
| Password | `bachir2023` |

These credentials are provided for demonstration and testing only. Do not use them for real or sensitive data.

## Data Files

The application uses the following Excel workbooks:

- `Clients.xlsx` — customer records.
- `Fournisseurs.xlsx` — supplier records.
- `Inventaire_Template.xlsx` — inventory data.
- `Journal.xlsx` — stock movement history.

Some filenames are retained in French because the existing application code and packaged JAR depend on those exact names. Keep the workbooks alongside the JAR or in the working directory when running the application.

**Usage note:** In the purchase and sales screens, press Enter once after each entry or reference selection.

## API Documentation

Generated Java API documentation is available in [`Documentation/apidocs/`](Documentation/apidocs/).
