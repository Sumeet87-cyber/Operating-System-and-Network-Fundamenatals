# Operating-System-and-Network-Fundamenatals
Here is project Summary of Cybersecurity and Ethical Hacking Internship Lab 1 Linux User Management & ACL Permission Configuration in Kali Linux.


🔐 Linux User Management & ACL Permission Configuration

This project focuses on fundamental Linux system administration tasks, specifically user management, directory permission handling, and Access Control List (ACL) configuration. The practical exercises are divided into two labs, each demonstrating essential security operations used by system administrators to control access to files and directories at a granular level.

📌 Lab 1: User Management and ACL Implementation

The first lab begins with saving a target file into the home directory or any temporary working folder. The objective is to secure this file using Linux ACLs while assigning appropriate permissions to multiple users.

1. Creating User Accounts & Project Directory

A new user account is created for Mr. Penney Johnson, followed by creating a project directory. The provided file is moved into this directory so it can later be managed through ACL permissions.

2. Installing and Using ACL

The ACL package (commonly acl on Debian/Kali) is installed to enable fine-grained permission control beyond standard Linux file modes.
ACL commands such as setfacl and getfacl are used to assign and verify permissions.

3. Restricting File Access

The file is secured by restricting default access so that unauthorized users cannot read or modify it. ACL rules are applied to precisely define who can interact with the file.

4. Testing Permissions with Multiple Users

A new user named testuser is created. When switching to this user, the test confirms that the file cannot be accessed due to restricted ACL settings.
Later, switching to pjohnson (Penney Johnson) verifies that the assigned permissions allow him to access the file as intended.
This demonstrates successful implementation of controlled access using ACL.

📌 Lab 2: Group Permissions & Multi-User Access Rules

Lab 2 expands the permission management tasks by involving multiple users and groups, especially for managing regional folder structures like Gujarat, Delhi, and Goa.

1. Creating Users & Assigning Passwords

Three users — Stefi, Aravind, and Jignesh — are created. Each user is assigned a common password (“India”) for simplicity.

2. Creating Group and Assigning Access

A new group named Citizen is created. All three users are added to this group, and group-level permissions (read, write, execute) are granted for a downloads directory so that all members can access shared content.

3. Applying Region-Based Permissions

Different permission rules are applied for regional directories:

a. Gujarat

    Jignesh receives full access.

    Aravind receives read + execute only.

b. Delhi

    Stefi is denied access completely.

c. Goa

    All Citizens are given full access.

    Subdirectories such as Goa/Anjuna and Goa/Candolim are edited with specific ACL rules based on the use case.

4. Final Verification

All assigned permissions (Gujarat, Delhi, Goa) are verified using getfacl to ensure ACL rules are correctly applied across users and directories.

✅ Conclusion

Both labs demonstrate essential Linux administrative skills, including user creation, group management, and precise permission control using ACLs. These exercises reflect real-world scenarios where system administrators must manage file security and user access efficiently to maintain system integrity.
