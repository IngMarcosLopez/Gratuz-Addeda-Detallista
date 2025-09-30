
# 🧾 Addenda Detallista - NetSuite SuiteApp

> A comprehensive NetSuite SuiteApp for managing Mexican retailer addenda in electronic invoicing processes.

[![Version](https://img.shields.io/badge/version-0.0.1-blue.svg)](package.json)
[![NetSuite](https://img.shields.io/badge/NetSuite-SuiteApp-orange.svg)](https://www.netsuite.com/)
[![Mexican Localization](https://img.shields.io/badge/Localization-Mexico-green.svg)](src/manifest.xml)

## 📋 Overview

**Addenda Detallista** is a specialized NetSuite SuiteApp designed to handle Mexican retailer addenda requirements for electronic invoicing. This application extends NetSuite's capabilities to comply with Mexican fiscal regulations and retailer-specific requirements for electronic document exchange.

### 🎯 Key Features

- **Electronic Invoice Integration**: Seamless integration with Mexican electronic invoicing systems
- **Retailer Addenda Management**: Comprehensive handling of retailer-specific addenda requirements
- **Custom Transaction Fields**: Extended transaction fields for Mexican compliance
- **Multi-Language Support**: Built-in support for Mexican localization
- **Automated Compliance**: Ensures adherence to Mexican fiscal regulations

## 🏗️ Architecture

This SuiteApp is built on NetSuite's SuiteCloud platform and includes:

### 📁 Core Components

```
src/
├── Objects/
│   ├── CustomLists/          # Predefined value lists for Mexican compliance
│   ├── TransactionBodyFields/ # Extended transaction fields
│   └── customSubtabs/        # Custom UI tabs
├── InstallationPreferences/   # Deployment configuration
├── manifest.xml              # App metadata and dependencies
└── deploy.xml                # Deployment specifications
```

### 🔧 Custom Lists

The application includes 24+ custom lists covering:

- **Tax Categories & Types**: Mexican tax classification systems
- **Currency Functions**: Multi-currency support with ISO codes
- **Document Status**: Electronic document lifecycle management
- **Payment Terms**: Mexican-specific payment term configurations
- **Special Services**: Retailer addenda service types
- **Transport & Logistics**: Shipping and delivery classifications

### 📊 Transaction Fields

Enhanced transaction records with 20+ custom fields including:

- GLN (Global Location Numbers) for buyers and sellers
- Purchase order references and dates
- Discount and charge calculations
- Special instruction handling
- Document status tracking

## 🚀 Installation

### Prerequisites

- NetSuite account with SuiteApp installation privileges
- Required NetSuite features (see [Dependencies](#dependencies))
- Mexican localization bundle: `com.netsuite.gratuzmxlocalizacion`

### Dependencies

This SuiteApp requires the following NetSuite features:

| Feature | Required | Purpose |
|---------|----------|---------|
| ASSEMBLIES | Optional | Assembly item management |
| INVENTORY | Optional | Inventory tracking |
| ACCOUNTING | Optional | Financial reporting |
| CUSTOMTRANSACTIONS | Optional | Custom transaction types |
| RECEIVABLES/PAYABLES | Optional | AR/AP management |

### Deployment

1. **Clone or download** this repository to your local development environment
2. **Configure** your NetSuite environment credentials
3. **Deploy** using SuiteCloud CLI:

```bash
# Install dependencies
npm install

# Run tests
npm test

# Deploy to NetSuite
suitecloud project:deploy
```

## 🧪 Testing

The project includes comprehensive Jest-based unit tests:

```bash
# Run all tests
npm test

# Run specific test file
npm test __tests__/sample-test.js
```

### Test Coverage

- NetSuite record operations
- Custom field validations
- Business logic verification
- Mock NetSuite modules for isolated testing

## 🔧 Development

### Project Structure

```
├── __tests__/           # Jest unit tests
├── src/                 # Source code
├── jest.config.js       # Jest configuration
├── suitecloud.config.js # SuiteCloud CLI configuration
└── package.json         # Node.js dependencies
```

### Configuration Files

- **`suitecloud.config.js`**: Configures SuiteCloud CLI with automated testing
- **`jest.config.js`**: Jest testing framework configuration
- **`jsconfig.json`**: JavaScript/TypeScript configuration for better IDE support

### Pre-deployment Testing

The application automatically runs unit tests before deployment to ensure code quality and prevent deployment of broken functionality.

## 📋 Compliance

This SuiteApp ensures compliance with:

- **SAT (Mexican Tax Authority)** electronic invoicing requirements
- **CFDI (Comprobante Fiscal Digital)** standards
- **Retailer-specific addenda** formats and requirements
- **Mexican localization** standards for NetSuite

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

### Development Guidelines

- Follow NetSuite SuiteScript best practices
- Maintain test coverage above 80%
- Update documentation for new features
- Ensure Mexican compliance requirements are met

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🆘 Support

For support and questions:

- **Documentation**: Check NetSuite SuiteCloud documentation
- **Issues**: Open an issue in this repository
- **Mexican Compliance**: Consult with your tax advisor for specific requirements

## 🔗 Related Resources

- [NetSuite SuiteCloud Platform](https://www.netsuite.com/portal/platform/developer/suitecloud-platform.shtml)
- [Mexican Electronic Invoicing (SAT)](https://www.sat.gob.mx/)
- [SuiteCloud CLI Documentation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1543970969.html)

---

**Made with ❤️ for Mexican NetSuite implementations**
