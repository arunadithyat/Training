# Training
Training for Team

Day 1 - Saturday 20/09/2025

Day 2 - Saturday 20/09/2026

Day 3 - None

Day 4 

<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Work Orders & Job Cards</title>
<link href="https://cdn.jsdelivr.net/npm/@mdi/font@6.5.95/css/materialdesignicons.min.css" rel="stylesheet">
<script src="https://cdn.tailwindcss.com"></script>
<style>
  @import url('https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&display=swap');
  body { font-family: 'Inter', sans-serif; background: #f1f5f9; color: #1e293b; }
  .dashboard-container { background: #fff; border-radius: 2rem; padding: 2.5rem; box-shadow: 0 10px 30px rgba(0,0,0,0.05); }
  .work-order-grid { display: grid; gap: 1.5rem; grid-template-columns: repeat(auto-fill, minmax(280px, 1fr)); }
  .work-order-card { background: #ffffff; border-radius: 1rem; padding: 1.5rem; box-shadow: 0 4px 12px rgba(0,0,0,0.05); transition: transform 0.2s ease, box-shadow 0.2s ease; cursor: pointer; }
  .work-order-card:hover { transform: translateY(-5px); box-shadow: 0 8px 20px rgba(0,0,0,0.1); }
  .status-badge { padding: 0.3rem 0.8rem; border-radius: 9999px; font-weight: 600; text-transform: capitalize; font-size: 0.875rem; }
  .status-badge.pending { background-color: #fcd34d; color: #92400e; }
  .status-badge.wip { background-color: #60a5fa; color: #1e40af; }
  .status-badge.completed { background-color: #34d399; color: #065f46; }
  .status-badge.not-started { background-color: #cbd5e1; color: #475569; }
  .filter-button { background-color: #4f46e5; transition: all 0.3s ease; color: white; padding: 0.75rem 1.5rem; border-radius: 0.75rem; font-weight: 600; box-shadow: 0 4px 6px rgba(0,0,0,0.1); }
  .filter-button:hover { background-color: #4338ca; transform: translateY(-2px); box-shadow: 0 6px 8px rgba(0,0,0,0.15); }
  .filter-button:active { transform: translateY(0); box-shadow: 0 2px 4px rgba(0,0,0,0.1); }
  .loading-spinner { border: 4px solid rgba(0,0,0,0.1); border-left-color: #4f46e5; border-radius: 50%; width: 2rem; height: 2rem; animation: spin 1s linear infinite; }
  @keyframes spin { 0% { transform: rotate(0deg); } 100% { transform: rotate(360deg); } }
  .modal-overlay { position: fixed; top: 0; left: 0; width: 100%; height: 100%; background-color: rgba(0,0,0,0.6); display: flex; justify-content: center; align-items: center; z-index: 1000; }
  /* .modal-content { background: #fff; padding: 2.5rem; border-radius: 1.5rem; max-width: 650px; width: 90%; box-shadow: 0 15px 35px rgba(0,0,0,0.3); transition: transform 0.3s ease; }
  .job-card-item { cursor: pointer; padding: 0.5rem 0.75rem; border-radius: 0.5rem; margin-bottom: 0.25rem; transition: all 0.2s ease; } */
  .job-card-item:hover { background-color: #eef2ff; }
  .job-card-item.selected { background-color: #4f46e5; color: #fff; font-weight: 600; transform: translateY(-2px); box-shadow: 0 2px 6px rgba(0,0,0,0.1); }
  #statusMessage { transition: all 0.3s ease-in-out; }
  .material-message {
    transition: all 0.3s ease-in-out;
  }

  This is new logic I am extending the code with the help of LLM's and AI

  That’s awesome 🚀 — using LLMs/AI to extend logic into your workflow can save a lot of trial and error.

From what I see in your screenshot, you’re already experimenting, but Git is very syntax-sensitive — one small keyword like adding remote in the wrong place breaks the push. AI can definitely help here by:

Explaining errors in plain English (like why git push remote origin fails).

Suggesting corrected commands (git push origin main).

Automating fixes by checking if a remote exists, if credentials are set, etc.

Generating scripts/workflows that wrap Git commands and avoid common mistakes. 1
