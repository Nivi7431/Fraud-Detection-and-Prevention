The Legal Document System is a Python-based desktop application designed to manage legal documents and evidences efficiently and securely. It incorporates Knapsack Problem, Hashing, and B+ Tree concepts for document organization, evidence packaging, and search optimization.

Features
1. User Authentication
Signup and Login: Users can create accounts and log in to access their personal dashboard.
Secure access ensures that each user can only manage their own documents and evidences.

2. Document Management
Upload Documents: Securely upload legal documents with integrity checks.
View Document Integrity: Verify document integrity using SHA-256 hashing to detect unauthorized modifications.
Download and Delete: Download a copy of the document or delete it (if you are the owner).

3. Evidence Packaging with Knapsack Algorithm
Upload evidences with assigned urgency levels (1–10).
Automatically group evidences into packs using the Knapsack Problem concept. Each pack is filled up to a set capacity (e.g., 3 items per pack) with priority given to urgency levels.

4. B+ Tree for Document Management
A B+ Tree is used to efficiently organize and retrieve documents by name.
Supports sorted insertion and deletion for maintaining an ordered list of documents.

5. Search Functionality
Case-insensitive search to quickly find documents by name using the B+ Tree structure.

Concepts Implemented
1. Knapsack Problem:
Used to organize evidences into packs based on urgency and capacity.
Ensures that evidences with higher urgency are prioritized in packing.
2. Hashing:
Documents are hashed using the SHA-256 algorithm for integrity verification.
Detects any modifications made to a document by comparing the hash before and after viewing.
3. B+ Tree:
Handles document indexing for efficient searching and retrieval.
Maintains a sorted structure, allowing dynamic updates (insertions and deletions).
