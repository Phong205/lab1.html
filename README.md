<!DOCTYPE html>
<html lang="vi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="styles.css">
    <title>Đăng Ký Tài Khoản</title>
</head>
<body>
    <div class="container">
        <h1>Đăng Ký Tài Khoản</h1>
        <form id="registration-form">
            <div class="form-group">
                <label for="username">Username <span class="required">*</span></label>
                <input type="text" id="username" placeholder="Enter your username." required>
                <span class="error-message" id="username-error"></span>
            </div>

            <div class="form-group">
                <label for="password">Password <span class="required">*</span></label>
                <input type="password" id="password" placeholder="Enter your password." required>
                <button type="button" id="toggle-password">Show/Hide</button>
                <span class="error-message" id="password-error"></span>
            </div>

            <div class="form-group">
                <label for="email">Email Address <span class="obligatory">(Obligatory)</span></label>
                <input type="email" id="email" placeholder="Enter your email.">
                <span class="error-message" id="email-error"></span>
            </div>

            <div class="form-group">
                <label for="full-name">Full Name <span class="obligatory">(Obligatory)</span></label>
                <input type="text" id="full-name" placeholder="Enter your full name.">
            </div>

            <div class="form-group">
                <label for="role">Role <span class="required">*</span></label>
                <select id="role" required>
                    <option value="">Select your role</option>
                    <option value="admin">Admin</option>
                    <option value="user">User</option>
                </select>
                <span class="error-message" id="role-error"></span>
            </div>

            <div class="form-group">
                <label for="profile-picture">Profile Picture <span class="optional">(Optional)</span></label>
                <input type="file" id="profile-picture" accept="image/*">
                <input type="url" id="profile-picture-url" placeholder="Or enter image URL.">
                <div id="image-preview"></div>
            </div>

            <div class="form-group">
                <label>Account Created At:</label>
                <div id="created-at" class="read-only">2024-09-28</div>
            </div>

            <div class="form-group">
                <label>Last Updated At:</label>
                <div id="updated-at" class="read-only">2024-09-28</div>
            </div>

            <button type="submit" id="submit-button" disabled>Create Account</button>
            <button type="button" id="cancel-button">Cancel</button>
        </form>
    </div>
</body>
</html>
