- 👋 Hi, I’m @neerja-1984
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...

<!---
neerja-1984/neerja-1984 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->

---------------

## 🎵 Check Out My Music Player  
🎧[Listen Here!](https://neerja-1984.github.io/music-player/)


------------------


<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Book Club Suggestion</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background-color: #f9f9f9;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
    }
    form {
      background-color: white;
      padding: 40px;
      border-radius: 10px;
      box-shadow: 0 10px 30px rgba(0,0,0,0.1);
      max-width: 400px;
      width: 100%;
    }
    h1 {
      color: #333;
    }
    label {
      display: block;
      margin-top: 10px;
    }
    input, textarea, button {
      width: 100%;
      margin-top: 8px;
      padding: 12px;
      font-size: 14px;
      border: 1px solid #ccc;
      border-radius: 8px;
    }
    button {
      background-color: #007bff;
      color: white;
      cursor: pointer;
      margin-top: 20px;
    }
    button:hover {
      background-color: #0056b3;
    }
  </style>
</head>
<body>
  <form id="suggestion-form">
    <h1>📚 Book Club Suggestions</h1>
    <label for="title">Book Title:</label>
    <input type="text" id="title" required />

    <label for="author">Author:</label>
    <input type="text" id="author" required />

    <label for="reason">Why do you recommend it?</label>
    <textarea id="reason" rows="5" required></textarea>

    <button type="submit">Submit Suggestion</button>
  </form>

  <script>
    document.getElementById('suggestion-form').addEventListener('submit', function(e) {
      e.preventDefault();
      
      const title = encodeURIComponent(document.getElementById('title').value);
      const author = encodeURIComponent(document.getElementById('author').value);
      const reason = encodeURIComponent(document.getElementById('reason').value);

      // GitHub Issue URL with pre-filled data
      const githubUsername = 'your-username';
      const repoName = 'your-repo';
      const issueURL = `https://github.com/${githubUsername}/${repoName}/issues/new?title=Book%20Suggestion:%20${title}&body=**Book%20Title:**%20${title}%0A**Author:**%20${author}%0A**Reason:**%20${reason}`;
      
      window.location.href = issueURL;
    });
  </script>
</body>
</html>
