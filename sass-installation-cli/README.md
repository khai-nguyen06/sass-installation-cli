# sass-installation-cli

Thực hành cài đặt và sử dụng SASS CLI.

## Bước 1: Cài SASS toàn cục

```bash
node -v
npm -v
npm install -g sass
sass -v
```

Nếu PowerShell báo lỗi `running scripts is disabled on this system`, mở PowerShell với quyền Administrator và chạy:

```powershell
Set-ExecutionPolicy RemoteSigned -Scope CurrentUser
```

Gõ `Y` rồi nhấn Enter.

## Bước 2: Biên dịch SCSS

Dùng SASS cài toàn cục:

```bash
sass scss/styles.scss css/styles.css            # biên dịch một lần
sass --watch scss/styles.scss css/styles.css    # tự biên dịch khi lưu file
```

Hoặc dùng npm script (cần `npm install` trước):

```bash
npm run build
npm run watch
```

Sau đó mở `index.html` trong trình duyệt.

## Cấu trúc thư mục

```
sass-installation-cli/
├── scss/
│   ├── _variables.scss
│   └── styles.scss
├── css/
│   └── styles.css     # sinh ra khi biên dịch
├── index.html
└── package.json
```
