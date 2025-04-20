<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <title>Гифки и Текст</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            max-width: 800px;
            margin: 20px auto;
            padding: 20px;
        }
        .post-form {
            border: 2px solid #ddd;
            padding: 20px;
            margin-bottom: 30px;
        }
        .posts-container {
            display: grid;
            gap: 20px;
        }
        .post {
            border: 1px solid #eee;
            padding: 15px;
            border-radius: 8px;
            box-shadow: 0 2px 4px rgba(0,0,0,0.1);
        }
        input, textarea {
            width: 100%;
            margin: 10px 0;
            padding: 8px;
        }
        button {
            background: #4CAF50;
            color: white;
            padding: 10px 20px;
            border: none;
            cursor: pointer;
        }
    </style>
</head>
<body>
    <div class="post-form">
        <h2>Создать пост</h2>
        <input type="file" id="gifInput" accept="image/gif">
        <textarea id="textInput" placeholder="Введите текст..." rows="4"></textarea>
        <button onclick="addPost()">Добавить пост</button>
    </div>

    <div class="posts-container" id="postsContainer"></div>

    <script>
        // Локальное хранилище для постов
        let posts = JSON.parse(localStorage.getItem('posts')) || [];

        // Функция добавления поста
        function addPost() {
            const fileInput = document.getElementById('gifInput');
            const text = document.getElementById('textInput').value;

            if (!fileInput.files[0] && !text) {
                alert('Добавьте гифку или текст!');
                return;
            }

            // Чтение гифки
            const reader = new FileReader();
            reader.onload = function(e) {
                const newPost = {
                    gif: e.target.result,
                    text: text,
                    date: new Date().toLocaleString()
                };

                posts.push(newPost);
                localStorage.setItem('posts', JSON.stringify(posts));
                renderPosts();
            };

            if (fileInput.files[0]) {
                reader.readAsDataURL(fileInput.files[0]);
            } else {
                reader.onload({ target: { result: null } });
            }
        }

        // Отображение постов
        function renderPosts() {
            const container = document.getElementById('postsContainer');
            container.innerHTML = posts.map((post, index) => 
                <div class="post">
                    ${post.gif ? <img src="${post.gif}" style="max-width: 300px; display: block; margin-bottom: 10px;"> : ''}
                    <p>${post.text}</p>
                    <small>${post.date}</small>
                </div>
            ).join('');
        }

        // Первая загрузка
        renderPosts();
    </script>
</body>
</html>
