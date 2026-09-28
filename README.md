# offlinePos
OfflinePOS is an open-source, offline-first Inventory Management and Point of Sale system for small businesses and retail shops. Manage products, stock, sales, purchases, customers, suppliers, billing, payments, and reports locally without requiring a constant internet connection.
# OfflinePOS

**Offline-first Inventory Management & Point of Sale system for small businesses.**

OfflinePOS is an open-source desktop application designed to help small shops and businesses manage inventory, sales, purchases, customers, suppliers, billing, and business reports — even when there is no internet connection.

## ✨ Features

### 🧾 Point of Sale

* Fast product search
* Barcode scanning
* Shopping cart
* Discounts
* Tax/GST support
* Cash, UPI, card and other payment methods
* Split payments
* Hold and resume bills
* Sales returns and refunds
* Invoice generation
* Thermal printer support

### 📦 Inventory

* Product management
* Categories and brands
* SKU and barcode support
* Stock tracking
* Stock adjustments
* Low-stock alerts
* Inventory movements
* Batch and expiry tracking

### 🛒 Purchases

* Supplier management
* Purchase invoices
* Purchase returns
* Automatic stock updates
* Supplier ledger

### 👥 Customers

* Customer profiles
* Purchase history
* Credit management
* Customer ledger
* Payment history

### 📊 Reports

* Daily and monthly sales
* Product-wise sales
* Profit reports
* Inventory valuation
* Low-stock reports
* Purchase reports
* Customer outstanding
* Supplier outstanding
* Tax/GST reports

### 🔐 Security

* User authentication
* Role-based permissions
* Owner, Admin, Manager and Cashier roles
* Audit logs
* Local database
* Backup and restore

## 📴 Offline First

OfflinePOS is designed around an offline-first architecture.

Core operations such as:

* Billing
* Inventory management
* Product management
* Sales
* Purchases
* Reports

work locally without requiring an internet connection.

Internet connectivity can optionally be used for future features such as cloud backup, synchronization and remote reporting.

## 🛠️ Tech Stack

* **Desktop:** Tauri
* **Frontend:** React
* **Language:** TypeScript
* **Native layer:** Rust
* **Database:** SQLite
* **ORM:** Drizzle ORM
* **Styling:** Tailwind CSS
* **UI:** shadcn/ui
* **State Management:** Zustand
* **Validation:** Zod
* **Testing:** Vitest + Playwright
* **CI/CD:** GitHub Actions
* **Package Manager:** pnpm

## 🏗️ Architecture

```text
React + TypeScript
        │
        ▼
     Tauri
        │
        ▼
 Rust Application Layer
        │
        ▼
      SQLite
```

The architecture is designed so that optional cloud synchronization can be added without making the core POS dependent on the internet.

## 📁 Project Structure

```text
apps/
  desktop/
    src/
    src-tauri/

packages/
  database/
  shared/
  validation/
  ui/

docs/
tests/
scripts/

.github/
  workflows/
  ISSUE_TEMPLATE/
```

## 🚀 Getting Started

### Requirements

* Node.js
* pnpm
* Rust
* Tauri prerequisites

### Clone

```bash
git clone https://github.com/Cw-shubhamdubey/offline-pos.git
cd offline-pos
```

### Install dependencies

```bash
pnpm install
```

### Start development

```bash
pnpm tauri dev
```

### Build

```bash
pnpm tauri build
```

## 🗃️ Database

OfflinePOS uses SQLite as its primary local database.

The database contains modules for:

```text
Users
Products
Categories
Inventory
Sales
Sale Items
Payments
Purchases
Customers
Suppliers
Returns
Expenses
Tax Rates
Audit Logs
Backups
```

Database migrations are version controlled so that installations can be upgraded safely.

## 🗺️ Roadmap

### Phase 1

* [ ] Project foundation
* [ ] SQLite database
* [ ] Authentication
* [ ] Product management

### Phase 2

* [ ] Inventory management
* [ ] Barcode support
* [ ] POS billing
* [ ] Payments
* [ ] Invoice printing

### Phase 3

* [ ] Customers
* [ ] Suppliers
* [ ] Purchases
* [ ] Returns
* [ ] Ledgers

### Phase 4

* [ ] Reports
* [ ] Backup and restore
* [ ] Hardware support

### Future

* [ ] Cloud synchronization
* [ ] Multi-store support
* [ ] Remote dashboard
* [ ] Mobile companion
* [ ] Public API
* [ ] Plugin system

## 🤝 Contributing

Contributions are welcome.

Before submitting a pull request:

1. Create an issue or discuss the change.
2. Fork the repository.
3. Create a feature branch.
4. Make your changes.
5. Add or update tests.
6. Submit a pull request.

Please read `CONTRIBUTING.md` for detailed guidelines.

## 🔒 Security

If you discover a security vulnerability, please follow the instructions in `SECURITY.md` rather than publicly disclosing the vulnerability.

## 📄 License

This project will be released under an open-source license. See `LICENSE` for details.

## 👨‍💻 Maintainer

**Shubham Dubey**

GitHub: `@Cw-shubhamdubey`

---

> OfflinePOS is being built to provide a simple, reliable and privacy-friendly POS experience for small businesses, especially in environments where internet connectivity cannot be guaranteed.
