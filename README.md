# **Webflow CMS to Sanity Migration Tool**

This tool assists users in migrating their Webflow content to Sanity. It fetches collections from Webflow and allows users to select which site and collection they wish to migrate. After selection, the tool maps Webflow items to a predefined Sanity schema, provided by the user, and uploads them to Sanity.

This code contains a demo mapping function for how to handle:

1. Migrating images from Webflow to Sanity.
2. Migrating files from Webflow to Sanity.
3. Migrating Webflow Rich Text Content (HTML) to Sanity Block Content.

## **Prerequisites**

- Node.js
- **`node-fetch`**, **`axios`**, **`readline`**, **`@sanity/client`**, **`@sanity/block-tools`**, **`@sanity/schema`**, **`jsdom`**, and **`dotenv`** npm packages.
- Webflow API Key
- Sanity Project ID, Dataset Name, and Sanity Token

## **Setup**

1. Clone the repository.

   ```bash
   git clone <repository-url>
   ```

2. Navigate to the project directory.

   ```bash
   cd path-to-directory
   ```

3. Install the required `npm` packages.

   ```bash
   npm install
   ```

4. Setup your environment variables:

   Create a **`.env`** file in the root directory and populate it with your Webflow API Key, Sanity Project ID, Dataset Name, and Sanity Token.

   ```makefile
   WEBFLOW_API_KEY=YOUR_WEBFLOW_API_KEY
   SANITY_PROJECT_ID=YOUR_SANITY_PROJECT_ID
   SANITY_DATASET=YOUR_SANITY_DATASET_NAME
   SANITY_TOKEN=YOUR_SANITY_TOKEN
   ```

## **Usage**

1. Run the script.

   ```bash
   node path-to-your-script.js
   ```

2. Follow the on-screen prompts to select a Webflow site and collection.
3. Wait for the content to be migrated. The tool will print progress messages as it processes each item.

## **Features**

- Fetch all Webflow sites associated with the provided API key.
- Allow users to select which site and collection they wish to migrate from Webflow.
- Map Webflow content to a predefined Sanity schema.
- Handle image and file uploads to Sanity.
- Report any errors that occur during the migration process.

## **Notes**

- Ensure you have appropriate permissions for both Webflow and Sanity platforms.
- It's recommended to run a test migration on a smaller dataset or backup your Sanity dataset before performing a large-scale migration.

## **License**

This project is licensed under the MIT License.

---

You can customize the README further as per your needs.
