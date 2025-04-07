# Taseen's Legislative AI Tool

A web application that helps users analyze and search for legislative bills using AI. This tool has two main features:

1. **Bill Summarizer**: Upload a PDF of a legislative bill to get a comprehensive analysis
2. **Bill Searcher**: Search for information about a bill by name, number, state, etc.

## Project Structure

- Frontend: Hosted on GitHub Pages
- Backend: API server hosted on Render

## Setup Instructions

### Frontend (GitHub Pages)

1. Your repository is already configured to serve the frontend files from the main branch
2. Any changes pushed to the main branch will automatically update your site
3. The site will be available at: `https://[your-username].github.io/legislative-AI-reader/`

### Backend (Render)

1. Create a new Web Service on Render
2. Connect your GitHub repository
3. Configure the following settings:
   - **Name**: legislative-ai-reader-backend (or any name you prefer)
   - **Root Directory**: backend
   - **Runtime**: Node
   - **Build Command**: `npm install`
   - **Start Command**: `node server.js`
4. Add the following environment variables:
   - `OPENAI_API_KEY`: Your OpenAI API key
   - `PORT`: 10000 (or any port you prefer)
   - `FRONTEND_URL`: Your GitHub Pages URL (e.g., `https://[your-username].github.io/legislative-AI-reader`)

5. Deploy the service

6. Once deployed, copy the service URL (e.g., `https://legislative-ai-reader-backend.onrender.com`)

7. Update the `API_BASE_URL` constant in the frontend's `script.js` file to point to your Render service URL

## Usage

1. Navigate to your GitHub Pages URL
2. Select either the "Bill Summarizer" or "Bill Searcher" tab
3. For the summarizer, upload a PDF of a legislative bill
4. For the searcher, enter bill details and search for information

## Technologies Used

- Frontend: HTML, CSS, JavaScript
- Backend: Node.js, Express
- AI Processing: OpenAI GPT-4o-mini

## License

MIT
