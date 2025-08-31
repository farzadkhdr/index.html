<!DOCTYPE html>
<html lang="ku" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>سیستەمی پیشاندانی ناوەکان</title>
    <style>
        :root {
            --primary: #4361ee;
            --secondary: #3a0ca3;
            --success: #4cc9f0;
            --light: #f8f9fa;
            --dark: #212529;
            --gray: #6c757d;
        }
        
        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }
        
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background: linear-gradient(135deg, #f5f7fa 0%, #c3cfe2 100%);
            color: var(--dark);
            line-height: 1.6;
            padding: 20px;
            min-height: 100vh;
        }
        
        .container {
            max-width: 800px;
            margin: 0 auto;
            background: white;
            border-radius: 15px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
            padding: 30px;
            transition: transform 0.3s ease;
        }
        
        .container:hover {
            transform: translateY(-5px);
        }
        
        .system-title {
            color: var(--primary);
            margin-bottom: 25px;
            padding-bottom: 15px;
            border-bottom: 2px solid var(--primary);
            text-align: center;
            font-size: 28px;
        }
        
        .names-list {
            max-height: 400px;
            overflow-y: auto;
            border: 1px solid #eee;
            border-radius: 8px;
            padding: 15px;
            margin-bottom: 20px;
        }
        
        .name-item {
            padding: 12px 15px;
            border-bottom: 1px solid #eee;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        
        .name-item:last-child {
            border-bottom: none;
        }
        
        .name-text {
            font-weight: 600;
        }
        
        .code-text {
            color: var(--gray);
            font-size: 14px;
        }
        
        .timestamp {
            font-size: 12px;
            color: var(--gray);
        }
        
        .refresh-info {
            text-align: center;
            margin-top: 15px;
            color: var(--gray);
            font-size: 14px;
        }
        
        .empty-list {
            text-align: center;
            padding: 20px;
            color: var(--gray);
        }
        
        .controls {
            display: flex;
            justify-content: center;
            gap: 10px;
            margin-bottom: 20px;
        }
        
        .btn {
            background: var(--primary);
            color: white;
            border: none;
            padding: 10px 20px;
            border-radius: 8px;
            font-size: 14px;
            font-weight: 600;
            cursor: pointer;
            transition: background 0.3s;
        }
        
        .btn:hover {
            background: var(--secondary);
        }
    </style>
</head>
<body>
    <div class="container">
        <h2 class="system-title">سیستەمی پیشاندانی ناوەکان</h2>
        
        <div class="controls">
            <button class="btn" onclick="fetchNames()">نوێکردنەوەی لیستەکە</button>
            <button class="btn" onclick="clearNames()">سڕینەوەی هەموو ناوەکان</button>
        </div>
        
        <div class="names-list" id="namesList">
            <div class="empty-list">هیچ ناوێک تۆمارنەکراوە</div>
        </div>
        
        <div class="refresh-info">لیستەکە خۆکارانە هەموو ٥ چرکە جارێک نوێ دەبێتەوە</div>
    </div>

    <script>
        // وەرگرتنی ناوەکان لە localStorage
        function fetchNames() {
            try {
                const names = JSON.parse(localStorage.getItem('names')) || [];
                const namesList = document.getElementById('namesList');
                
                if (names.length === 0) {
                    namesList.innerHTML = '<div class="empty-list">هیچ ناوێک تۆمارنەکراوە</div>';
                    return;
                }
                
                namesList.innerHTML = '';
                
                names.forEach(item => {
                    const nameItem = document.createElement('div');
                    nameItem.className = 'name-item';
                    
                    const nameInfo = document.createElement('div');
                    
                    const nameText = document.createElement('div');
                    nameText.className = 'name-text';
                    nameText.textContent = item.name;
                    
                    const codeText = document.createElement('div');
                    codeText.className = 'code-text';
                    codeText.textContent = `کۆد: ${item.code}`;
                    
                    nameInfo.appendChild(nameText);
                    nameInfo.appendChild(codeText);
                    
                    const timestamp = document.createElement('div');
                    timestamp.className = 'timestamp';
                    
                    // دروستکردنی ڕێکەوتن و کات بە شێوازی کوردی
                    const date = new Date(item.timestamp);
                    const options = { 
                        year: 'numeric', 
                        month: '2-digit', 
                        day: '2-digit',
                        hour: '2-digit',
                        minute: '2-digit'
                    };
                    timestamp.textContent = date.toLocaleDateString('ar-KU', options);
                    
                    nameItem.appendChild(nameInfo);
                    nameItem.appendChild(timestamp);
                    
                    namesList.appendChild(nameItem);
                });
            } catch (error) {
                console.error('هەڵە لە وەرگرتنی زانیاریەکان:', error);
            }
        }
        
        // سڕینەوەی هەموو ناوەکان
        function clearNames() {
            if (confirm('دڵنیای لە سڕینەوەی هەموو ناوەکان؟')) {
                localStorage.removeItem('names');
                fetchNames();
                alert('هەموو ناوەکان سڕدرایەوە');
            }
        }
        
        // یەکەم جار لیستەکە پڕ دەکەینەوە
        fetchNames();
        
        // دانانی کاتی نوێکردنەوە بۆ هەموو 5 چرکە جارێک
        setInterval(fetchNames, 5000);
    </script>
</body>
</html>
