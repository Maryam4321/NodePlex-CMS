# NodePlex CMS
NodePlex CMS is a robust and flexible content management system built on Node.js, designed to provide a customizable and user-friendly environment for managing web content.

# Key Features
**User-Friendly Interface:** Includes a WYSIWYG editor, allowing non-technical users to manage content easily.

**Dynamic Site Structure:** Manage your site's structure with a tree-view GUI, templates, and drag-and-drop functionality.

**Integration Capable:** Seamlessly integrates with existing Node.js applications.

**Customizable:** Tailored to meet specific needs with extensive configuration options.

# Quick Start

# Getting Started
Follow these steps to set up NodePlex CMS quickly:

# Prerequisites
Install Node.js

Install MySQL

# Installation
**1. Create Project Directory:**
	mkdir mycms && cd mycms

**2. Install NodePlex CMS:**
	npm install cody

**3. Initialize Your Site:**
	node ./node_modules/cody/bin/create_site
Follow the interactive setup to configure your CMS.

**4. Configure DNS for Local Testing:**
	echo "127.0.0.1 mysite.local" | sudo tee -a /etc/hosts

**5. Start the Server:**
	node mysite.js
Alternatively, use forever for persistent running:
	forever start mysite.js

**6. Access Your Site:**
	CMS Dashboard: http://mysite.local:3001/en/dashboard
	Frontend: http://mysite.local:3001

# Configuration
Modify config.json directly or override settings using command-line flags or environment variables:
	node index.js -c my_config.json
	dbuser=admin dbpassword=secret port=8080 node index.js

# Troubleshooting
**Connection Errors:** Ensure MySQL is running. On macOS, use System Preferences to start MySQL. On Unix:
	mysqld &
 
**Authentication Errors:** If prompted unexpectedly for a password, check your MySQL root password and reset if necessary: MySQL Password Reset

# Contributors
We welcome contributions! See our contribution guidelines for more details.
