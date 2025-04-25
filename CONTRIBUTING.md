# Hướng dẫn Đóng góp

Cảm ơn bạn đã quan tâm đến việc đóng góp cho dự án này! Tài liệu này sẽ hướng dẫn bạn cách đóng góp một cách hiệu quả.

## Quy trình Đóng góp

1. **Fork repository**
   - Fork repository này về tài khoản GitHub của bạn
   - Clone repository đã fork về máy local

2. **Tạo branch mới**
   ```bash
   git checkout -b feature/ten-tinh-nang
   # hoặc
   git checkout -b fix/ten-loi
   ```

3. **Thực hiện thay đổi**
   - Thực hiện các thay đổi cần thiết
   - Đảm bảo code tuân thủ các quy tắc đã định

4. **Commit changes**
   - Sử dụng quy ước commit message chuẩn
   ```bash
   git commit -m "feat: add new feature"
   git commit -m "fix: resolve bug"
   ```

5. **Push changes**
   ```bash
   git push origin feature/ten-tinh-nang
   ```

6. **Tạo Pull Request**
   - Tạo Pull Request từ branch của bạn vào branch main
   - Mô tả chi tiết về thay đổi của bạn
   - Đính kèm screenshots nếu cần thiết

## Quy ước Commit Message

Sử dụng quy ước [Conventional Commits](https://www.conventionalcommits.org/):

```
<type>(<scope>): <description>

[optional body]

[optional footer(s)]
```

Các loại commit:
- `feat`: Thêm tính năng mới
- `fix`: Sửa lỗi
- `docs`: Thay đổi tài liệu
- `style`: Thay đổi về format
- `refactor`: Tái cấu trúc code
- `test`: Thêm hoặc sửa test
- `chore`: Cập nhật build tasks, package manager configs

### Ví dụ về Commit Message

1. **Thêm tính năng mới**
```
feat(auth): implement user authentication

- Add JWT token generation
- Add login endpoint
- Add middleware for token verification

Closes #123
```

2. **Sửa lỗi**
```
fix(api): resolve 500 error on user creation

The error was caused by missing validation for email format.
Added proper email validation using regex.

Fixes #456
```

3. **Cập nhật tài liệu**
```
docs(readme): update installation instructions

- Add new dependency requirements
- Update environment variables section
- Fix broken links
```

4. **Tái cấu trúc code**
```
refactor(api): improve error handling middleware

- Centralize error handling logic
- Add custom error types
- Improve error messages
```

5. **Cập nhật dependencies**
```
chore(deps): update dependencies to latest versions

- Update express to 4.18.2
- Update mongoose to 6.8.0
- Update jest to 29.3.1
```

6. **Thêm test**
```
test(auth): add unit tests for authentication

- Add tests for login endpoint
- Add tests for token generation
- Add tests for token verification
```

7. **Format code**
```
style(ui): format components with prettier

- Format all React components
- Update .prettierrc configuration
```

## Quy tắc Code

1. **Format code**
   - Sử dụng Prettier để format code
   - Tuân thủ ESLint rules

2. **Testing**
   - Viết test cho các tính năng mới
   - Đảm bảo tất cả test đều pass

3. **Documentation**
   - Cập nhật tài liệu khi cần thiết
   - Thêm comments cho code phức tạp

4. **Code Review**
   - Mọi Pull Request cần được review
   - Sửa các comment từ reviewer

## Cấu trúc Dự án

```
.
├── docs/           # Tài liệu
├── src/           # Source code
├── tests/         # Test files
├── .github/       # GitHub configurations
├── README.md      # Tài liệu chính
└── CONTRIBUTING.md # Hướng dẫn đóng góp
```

## Báo cáo Lỗi

Khi báo cáo lỗi, vui lòng cung cấp:
1. Mô tả chi tiết về lỗi
2. Các bước để tái tạo lỗi
3. Phiên bản đang sử dụng
4. Screenshots nếu cần thiết

## Yêu cầu Tính năng

Khi đề xuất tính năng mới, vui lòng:
1. Mô tả chi tiết về tính năng
2. Giải thích lý do cần thiết
3. Đề xuất cách triển khai

## Liên hệ

Nếu bạn có câu hỏi hoặc cần hỗ trợ:
- Mở issue trên GitHub
- Tham gia Discord/Slack channel
- Liên hệ qua email

## Giấy phép

Bằng cách đóng góp vào dự án này, bạn đồng ý rằng đóng góp của bạn sẽ được cấp phép theo giấy phép của dự án. 