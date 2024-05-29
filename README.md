- 👋 Hi, I’m @Zeyadmj
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...

<!---
Zeyadmj/Zeyadmj is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
<!DOCTYPE html>
<html lang="ar">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Gems - Zeyad Mandor Gaming</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-image: url('https://path-to-your-gaming-background-image.jpg'); /* ضع هنا رابط صورة الخلفية */
            background-size: cover;
            color: #fff;
            margin: 0;
            padding: 0;
        }

        header {
            text-align: center;
            padding: 20px;
            background-color: rgba(0, 0, 0, 0.5);
        }

        h1 {
            margin: 0;
            font-size: 2.5em;
        }

        #comments {
            margin: 50px auto;
            width: 80%;
            max-width: 800px;
            background-color: rgba(0, 0, 0, 0.7);
            padding: 20px;
            border-radius: 10px;
        }

        #comment-form {
            display: flex;
            flex-direction: column;
        }

        #comment-input {
            padding: 10px;
            border-radius: 5px;
            margin-bottom: 10px;
            resize: none;
        }

        button {
            padding: 10px;
            border-radius: 5px;
            background-color: #007BFF;
            color: white;
            border: none;
            cursor: pointer;
        }

        .comment {
            background-color: rgba(255, 255, 255, 0.1);
            padding: 10px;
            margin-top: 10px;
            border-radius: 5px;
        }
    </style>
</head>
<body>
    <header>
        <h1>Gems - Zeyad Mandor Gaming</h1>
    </header>
    <main>
        <section id="comments">
            <h2>التعليقات</h2>
            <div id="comment-section">
                <!-- التعليقات ستظهر هنا -->
            </div>
            <form id="comment-form">
                <textarea id="comment-input" placeholder="أضف تعليقك هنا..." required></textarea>
                <button type="submit">إرسال</button>
            </form>
        </section>
    </main>
    <script>
        document.getElementById('comment-form').addEventListener('submit', function(event) {
            event.preventDefault();

            let commentInput = document.getElementById('comment-input');
            let commentText = commentInput.value;

            if (commentText.trim() !== "") {
                let commentSection = document.getElementById('comment-section');
                let newComment = document.createElement('div');
                newComment.textContent = commentText;
                newComment.className = 'comment';

                commentSection.appendChild(newComment);
                commentInput.value = '';
            }
        });
    </script>
</body>
</html>
