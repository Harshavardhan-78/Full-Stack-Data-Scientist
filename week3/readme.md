Online Library Management System (Python + Supabase/Postgres)

This is a command-line library management system built in Python, with Supabase (Postgres) as the backend.
It simulates real-world operations like member registration, book management, borrowing, returning, and generating reports.

=> Features

👥 Member Management

Register new members (name & email).

List all registered members.

Update member email.

Delete members (only if they have no active borrowings).

📖 Book Management

Add new books with title, author, category, and stock.

List all books with availability.

Update book stock when new copies are added.

Delete books (only if not borrowed).

🔎 Search

Search books by title, author, or category.

🔄 Borrow & Return (Transactions)

Borrow a book: checks stock, decreases count, inserts borrow record.

Return a book: updates return date, increases stock, prevents double returns.

📊 Reports

Top borrowed books (via Supabase RPC).

Overdue books (borrowed >14 days, not returned).

Borrow count per member (via Supabase RPC).

🏗️ Tech Used

Python for CLI interface.

Supabase (Postgres) as database.

supabase-py SDK for queries.

dotenv for environment variables.
