# intellectia
## Your Guardian Against Misleading AI-Generated Content.

At Intellectia, we're on a mission to eliminate misinformation and AI-generated deception. Our vigilant system detects and removes misleading articles, thanks to the dedicated efforts of our user community. With human reviews ensuring accuracy, we're your trusted platform for truthful, transparent, and reliable content. Join us in the fight against misinformation!

🔗 **Useful Links:**

- 💬[Discord]: https://discord.gg/8vV4bjSh
- 📫[PostMan]: https://www.postman.com/galactic-firefly-721755/workspace/intellectia/request/10849501-459d4afa-6e15-4611-92e6-7d852344e17c

## Do we use AI?
Yes, we do utilize AI technology within our platform. We employ Large Language Models (LLMs) to enable our users to engage in conversations with `Intellectia` and seek answers to their questions. It's important to note that our AI system retrieves responses solely from our carefully curated database and knowledge base. These resources are comprised of trusted articles written by human experts and reviewed by human editors. We have a strict policy in place to exclude any content generated by AI algorithms.

The rationale behind this policy is to address concerns related to potential misinformation or inaccuracies that can arise from AI-generated content. LLMs, including those from OpenAI, have been known to generate persuasive yet factually incorrect information, which can lead to misunderstandings or inaccuracies. By relying exclusively on human-reviewed and curated content, we aim to ensure the highest level of accuracy and reliability in the information provided to our users.

Think of "Intellectia" as a vast library of knowledge that users can engage with through conversational interactions. We achieve this through the use of LLM technology, although it's important to clarify that we don't utilize OpenAI models specifically. Instead, we are considering the adoption of the "https://mistral.ai/news/announcing-mistral-7b/" technology, which appears to be a promising choice for our platform. This decision aligns with our commitment to delivering accurate and trustworthy information to our users while leveraging advanced AI tools to enhance their experience.

## Frequently Asked Questions

### Do we use AI?

Yes, we utilize AI technology within our platform to enhance user interactions and provide valuable information.

### How do we use AI?

We employ Large Language Models (LLMs) to enable our users to engage in conversations with "Intellectia" and seek answers to their questions. 

### What sources do we rely on for information?

Our AI system retrieves responses exclusively from our carefully curated database and knowledge base. These resources are comprised of trusted articles written by human experts and reviewed by human editors.

### Why do we exclude AI-generated content?

Our strict policy is to exclude any content generated by AI algorithms. This is due to concerns related to the potential generation of misinformation or inaccuracies by LLMs, including the generation of convincing yet factually incorrect information. By relying solely on human-reviewed and curated content, we aim to ensure the highest level of accuracy and reliability in the information provided to our users.

### What is the role of "Intellectia"?

Think of "Intellectia" as a vast library of knowledge that users can engage with through conversational interactions. 

### Which AI technology are we considering?

We are exploring the use of [Mistral 7B](https://mistral.ai/news/announcing-mistral-7b/), which shows promise as a suitable AI technology for our platform. This decision aligns with our commitment to delivering accurate and trustworthy information to our users while leveraging advanced AI tools to enhance their experience.


## Setup

**Project Setup Instructions**

1. **Clone the Repository**:
   ```
   git clone git@github.com:prasenjeet-symon/intellectia.git
   ```

2. **Navigate to the Project Directory**:
   ```
   cd intellectia/packages/server
   ```

3. **Install Dependencies**:
   ```
   npm install
   ```

4. **Database Configuration**:
   - Ensure you have XAMPP installed and running.
   - Create a MySQL database for your project in XAMPP. Note down the database name, username, and password.
   - Copy the `.env.example` file to a new file named `.env` in the `packages/server` directory.
   - Open the `.env` file and replace the placeholders with your MySQL database connection details
    
5. **Generate Prisma Client**:
   ```
   npx prisma generate
   ```

6. **Run Database Migrations**:
   ```
   npx prisma migrate dev
   ```
   This command will create database tables based on your Prisma schema and apply any pending migrations.

7. **Start the Development Server**:
   ```
   npm start
   ```
   This command uses `ts-node-dev` to run the TypeScript files in your `src` directory. It will automatically restart the server whenever you make changes to your code.

8. **Build the Project (Optional)**:
   ```
   npm run build
   ```
   If you want to create a production-ready build of your project, use this command. The output will be in the `dist` directory.

9. **Testing**:
   - Run your tests with the following command:
     ```
     npm test
     ```
     Modify the test script in your `package.json` file to specify your testing framework (e.g., Jest, Mocha).

By following these setup instructions, you'll have your Express project located at 'packages/server' connected to a MySQL database using XAMPP, with database migration capabilities using Prisma, and environment variables properly configured. Make sure to adapt the configuration and environment variables to your specific project requirements.
