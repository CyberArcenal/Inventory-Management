
# Developer Notes

## 🛠 Project Structure
- **/src** → main application source code
- **/db** → SQLite database files
- **/docs** → documentation (user guide, dev notes)
- **/assets** → images, icons, static resources

## ⚙️ Setup for Development
1. Clone the repository:
   ```bash
   git clone https://github.com/CyberArcenal/Inventory-Management.git
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Run in development mode:
   ```bash
   npm start
   ```

## 📦 Packaging
- Use **Electron Builder** for creating installers:
  ```bash
  npm run dist
  ```
- Output will be generated in the `/dist` folder.

## 🔒 Licensing & Activation
- Lite version: no license enforcement.
- Pro version: activation key required (handled via `license_key` table).
- Ensure audit-safe logging for license activation/deactivation.

## 🧩 Coding Standards
- Follow modular CRUD patterns.
- Enforce audit clarity in all transactions.
- Keep service layer abstraction clean and reusable.
- Use serializer patterns for consistent API responses.

## 🚀 Deployment Notes
- Works on Windows 10+.
- SQLite database is local by default.
- Optional: connect to external DB server for multi-branch setups.

## 📖 Contribution
- Fork the repo and create a feature branch.
- Submit pull requests with clear commit messages.
- Document any new modules or workflows in `/docs`.
