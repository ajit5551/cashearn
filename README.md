<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>EarnMoney - Make Money Online</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.10.0/font/bootstrap-icons.css">
    <style>
        :root {
            --primary-color: #6e8efb;
            --secondary-color: #a777e3;
        }
        body {
            background-color: #f8f9fa;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        .navbar-brand {
            font-weight: 700;
            font-size: 1.5rem;
        }
        .hero-section {
            background: linear-gradient(135deg, var(--primary-color), var(--secondary-color));
            color: white;
            padding: 5rem 0;
            border-radius: 0 0 20px 20px;
            margin-bottom: 3rem;
        }
        .card {
            border-radius: 15px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
            margin-bottom: 2rem;
            border: none;
        }
        .card-header {
            border-radius: 15px 15px 0 0 !important;
            background-color: #fff;
            border-bottom: 1px solid rgba(0,0,0,0.1);
        }
        .btn-primary {
            background-color: var(--primary-color);
            border: none;
            padding: 10px 25px;
            border-radius: 50px;
        }
        .btn-primary:hover {
            background-color: #5a7df4;
        }
        .feature-icon {
            font-size: 2.5rem;
            color: var(--primary-color);
            margin-bottom: 1rem;
        }
        .balance-card {
            background: linear-gradient(135deg, var(--primary-color), var(--secondary-color));
            color: white;
        }
        .form-control {
            border-radius: 50px;
            padding: 12px 20px;
        }
        .footer {
            background-color: #343a40;
            color: white;
            padding: 3rem 0;
            margin-top: 3rem;
        }
        .language-selector {
            position: fixed;
            bottom: 20px;
            right: 20px;
            z-index: 1000;
        }
        .language-btn {
            width: 40px;
            height: 40px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            cursor: pointer;
            margin-bottom: 10px;
            background: white;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
        }
        .currency {
            font-family: Arial, sans-serif;
        }
    </style>
</head>
<body>
    <!-- Navigation -->
    <nav class="navbar navbar-expand-lg navbar-dark bg-primary sticky-top">
        <div class="container">
            <a class="navbar-brand" href="#" data-i18n="app_name">EarnMoney</a>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarNav">
                <ul class="navbar-nav me-auto">
                    <li class="nav-item">
                        <a class="nav-link active" href="#" data-i18n="home">Home</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#" data-i18n="how_it_works">How It Works</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#" data-i18n="earnings">Earnings</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#" data-i18n="referrals">Referrals</a>
                    </li>
                </ul>
                <ul class="navbar-nav">
                    <li class="nav-item">
                        <a class="nav-link" href="login.html" data-i18n="login">Login</a>
                    </li>
                    <li class="nav-item">
                        <a class="btn btn-light ms-2" href="signup.html" data-i18n="signup">Sign Up</a>
                    </li>
                </ul>
            </div>
        </div>
    </nav>

    <!-- Hero Section -->
    <section class="hero-section text-center">
        <div class="container">
            <h1 class="display-4 fw-bold mb-4" data-i18n="hero_title">Start Earning Money Today</h1>
            <p class="lead mb-5" data-i18n="hero_subtitle">Join thousands of users who are making money with our platform. Simple, fast, and secure.</p>
            <a href="signup.html" class="btn btn-light btn-lg px-5 py-3" data-i18n="get_started">Get Started - It's Free</a>
        </div>
    </section>

    <!-- Features Section -->
    <section class="container">
        <div class="row text-center mb-5">
            <div class="col-md-4">
                <div class="feature-icon">
                    <i class="bi bi-cash-stack"></i>
                </div>
                <h3 data-i18n="feature1_title">Easy Earnings</h3>
                <p data-i18n="feature1_desc">Complete simple tasks and start earning money immediately.</p>
            </div>
            <div class="col-md-4">
                <div class="feature-icon">
                    <i class="bi bi-people-fill"></i>
                </div>
                <h3 data-i18n="feature2_title">Referral Program</h3>
                <p data-i18n="feature2_desc">Earn 20% of your referrals' earnings for life.</p>
            </div>
            <div class="col-md-4">
                <div class="feature-icon">
                    <i class="bi bi-shield-check"></i>
                </div>
                <h3 data-i18n="feature3_title">Secure Payments</h3>
                <p data-i18n="feature3_desc">Fast and secure withdrawals to your Indian bank account or UPI.</p>
            </div>
        </div>
    </section>

    <!-- Dashboard Page (example of logged-in view) -->
    <div id="dashboardPage" class="container py-5" style="display: none;">
        <div class="row">
            <div class="col-md-4">
                <div class="card balance-card text-white mb-4">
                    <div class="card-body text-center">
                        <h5 class="card-title" data-i18n="your_balance">Your Balance</h5>
                        <h2 class="card-text currency">₹1,250.50</h2>
                        <div class="d-flex justify-content-center mt-3">
                            <a href="deposit.html" class="btn btn-light me-2" data-i18n="deposit">Deposit</a>
                            <a href="withdraw.html" class="btn btn-outline-light" data-i18n="withdraw">Withdraw</a>
                        </div>
                    </div>
                </div>
                
                <div class="card mb-4">
                    <div class="card-header">
                        <h5 class="mb-0" data-i18n="quick_actions">Quick Actions</h5>
                    </div>
                    <div class="card-body">
                        <a href="#" class="btn btn-outline-primary w-100 mb-2" data-i18n="earn_money">Earn Money</a>
                        <a href="referrals.html" class="btn btn-outline-primary w-100 mb-2" data-i18n="refer_friends">Refer Friends</a>
                        <a href="#" class="btn btn-outline-primary w-100 mb-2" data-i18n="transaction_history">Transaction History</a>
                        <a href="#" class="btn btn-outline-primary w-100" data-i18n="settings">Settings</a>
                    </div>
                </div>
            </div>
            
            <div class="col-md-8">
                <div class="card mb-4">
                    <div class="card-header d-flex justify-content-between align-items-center">
                        <h5 class="mb-0" data-i18n="recent_activity">Recent Activity</h5>
                        <a href="#" class="small" data-i18n="view_all">View All</a>
                    </div>
                    <div class="card-body">
                        <ul class="list-group list-group-flush">
                            <li class="list-group-item d-flex justify-content-between align-items-center">
                                <div>
                                    <h6 class="mb-1" data-i18n="referral_bonus">Referral Bonus</h6>
                                    <small class="text-muted" data-i18n="today_1045am">Today, 10:45 AM</small>
                                </div>
                                <span class="text-success currency">+₹50.00</span>
                            </li>
                            <li class="list-group-item d-flex justify-content-between align-items-center">
                                <div>
                                    <h6 class="mb-1" data-i18n="task_completion">Task Completion</h6>
                                    <small class="text-muted" data-i18n="yesterday_330pm">Yesterday, 3:30 PM</small>
                                </div>
                                <span class="text-success currency">+₹25.50</span>
                            </li>
                            <li class="list-group-item d-flex justify-content-between align-items-center">
                                <div>
                                    <h6 class="mb-1" data-i18n="withdrawal">Withdrawal</h6>
                                    <small class="text-muted" data-i18n="may_12_2023">May 12, 2023</small>
                                </div>
                                <span class="text-danger currency">-₹500.00</span>
                            </li>
                        </ul>
                    </div>
                </div>
                
                <div class="card">
                    <div class="card-header">
                        <h5 class="mb-0" data-i18n="referral_program">Referral Program</h5>
                    </div>
                    <div class="card-body">
                        <div class="alert alert-info">
                            <strong data-i18n="earn_20_commission">Earn 20% commission</strong> <span data-i18n="referral_desc">on your referrals' earnings for life!</span>
                        </div>
                        <div class="input-group mb-3">
                            <input type="text" class="form-control" id="referralLink" value="https://earnmoney.com/ref/user123" readonly>
                            <button class="btn btn-primary" onclick="copyReferralLink()" data-i18n="copy">Copy</button>
                        </div>
                        <div class="row text-center">
                            <div class="col-md-4">
                                <h4>15</h4>
                                <p class="text-muted" data-i18n="referrals">Referrals</p>
                            </div>
                            <div class="col-md-4">
                                <h4 class="currency">₹875.50</h4>
                                <p class="text-muted" data-i18n="earned">Earned</p>
                            </div>
                            <div class="col-md-4">
                                <h4 class="currency">₹1,250.00</h4>
                                <p class="text-muted" data-i18n="lifetime">Lifetime</p>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>

    <!-- Withdraw Page -->
    <div id="withdrawPage" class="container py-5">
        <div class="row justify-content-center">
            <div class="col-md-8">
                <div class="card">
                    <div class="card-header">
                        <h3 class="mb-0" data-i18n="withdraw_funds">Withdraw Funds</h3>
                    </div>
                    <div class="card-body">
                        <div class="alert alert-info">
                            <span data-i18n="min_withdraw_info">Minimum withdrawal amount is ₹200. Processing time is 3-5 business days.</span>
                        </div>
                        <form>
                            <div class="mb-3">
                                <label for="withdrawAmount" class="form-label" data-i18n="amount">Amount (₹)</label>
                                <div class="input-group">
                                    <span class="input-group-text">₹</span>
                                    <input type="number" class="form-control" id="withdrawAmount" min="200" step="1" required>
                                    <button class="btn btn-outline-secondary" type="button" id="withdrawAll" data-i18n="withdraw_all">Withdraw All</button>
                                </div>
                                <div class="form-text" data-i18n="available_balance">Available balance: ₹1,250.50</div>
                            </div>
                            <div class="mb-3">
                                <label for="withdrawMethod" class="form-label" data-i18n="withdraw_method">Withdrawal Method</label>
                                <select class="form-select" id="withdrawMethod" required>
                                    <option value="" data-i18n="select_method">Select withdrawal method</option>
                                    <option value="upi" data-i18n="upi">UPI</option>
                                    <option value="bank_account" data-i18n="bank_account">Bank Account</option>
                                    <option value="paytm" data-i18n="paytm">Paytm</option>
                                </select>
                            </div>
                            <div id="withdrawDetails" class="mb-4">
                                <!-- Withdrawal details will be shown here based on selection -->
                            </div>
                            <button type="submit" class="btn btn-primary w-100 py-2" data-i18n="request_withdrawal">Request Withdrawal</button>
                        </form>
                    </div>
                </div>
            </div>
        </div>
    </div>

    <!-- Language Selector -->
    <div class="language-selector">
        <div class="language-btn" onclick="changeLanguage('en')">EN</div>
        <div class="language-btn" onclick="changeLanguage('hi')">हिं</div>
        <div class="language-btn" onclick="changeLanguage('mr')">मर</div>
    </div>

    <!-- Footer -->
    <footer class="footer">
        <div class="container">
            <div class="row">
                <div class="col-md-4">
                    <h5 data-i18n="app_name">EarnMoney</h5>
                    <p data-i18n="footer_desc">The easiest way to make money online. Join thousands of satisfied users today.</p>
                </div>
                <div class="col-md-2">
                    <h5 data-i18n="quick_links">Quick Links</h5>
                    <ul class="list-unstyled">
                        <li><a href="#" class="text-white" data-i18n="home">Home</a></li>
                        <li><a href="#" class="text-white" data-i18n="how_it_works">How It Works</a></li>
                        <li><a href="#" class="text-white" data-i18n="earnings">Earnings</a></li>
                        <li><a href="#" class="text-white" data-i18n="referrals">Referrals</a></li>
                    </ul>
                </div>
                <div class="col-md-2">
                    <h5 data-i18n="account">Account</h5>
                    <ul class="list-unstyled">
                        <li><a href="login.html" class="text-white" data-i18n="login">Login</a></li>
                        <li><a href="signup.html" class="text-white" data-i18n="signup">Sign Up</a></li>
                        <li><a href="#" class="text-white" data-i18n="forgot_password">Forgot password</a></li>
                    </ul>
                </div>
                <div class="col-md-4">
                    <h5 data-i18n="contact_us">Contact Us</h5>
                    <ul class="list-unstyled">
                        <li><i class="bi bi-envelope me-2"></i> support@earnmoney.com</li>
                        <li><i class="bi bi-telephone me-2"></i> +91 98765 43210</li>
                    </ul>
                    <div class="mt-3">
                        <a href="#" class="text-white me-2"><i class="bi bi-facebook"></i></a>
                        <a href="#" class="text-white me-2"><i class="bi bi-twitter"></i></a>
                        <a href="#" class="text-white me-2"><i class="bi bi-instagram"></i></a>
                        <a href="#" class="text-white"><i class="bi bi-linkedin"></i></a>
                    </div>
                </div>
            </div>
            <hr class="mt-4 bg-light">
            <div class="row">
                <div class="col-md-6">
                    <p class="mb-0">&copy; 2023 EarnMoney. <span data-i18n="all_rights">All rights reserved.</span></p>
                </div>
                <div class="col-md-6 text-md-end">
                    <a href="#" class="text-white me-3" data-i18n="privacy_policy">Privacy Policy</a>
                    <a href="#" class="text-white me-3" data-i18n="terms">Terms of Service</a>
                    <a href="#" class="text-white" data-i18n="faq">FAQ</a>
                </div>
            </div>
        </div>
    </footer>

    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js"></script>
    <script src="https://cdn.jsdelivr.net/npm/sweetalert2@11"></script>
    <script>
        // Language translations
        const translations = {
            'en': {
                'app_name': 'EarnMoney',
                'home': 'Home',
                'how_it_works': 'How It Works',
                'earnings': 'Earnings',
                'referrals': 'Referrals',
                'login': 'Login',
                'signup': 'Sign Up',
                'dashboard': 'Dashboard',
                'your_balance': 'Your Balance',
                'deposit': 'Deposit',
                'withdraw': 'Withdraw',
                'logout': 'Logout',
                'hero_title': 'Start Earning Money Today',
                'hero_subtitle': 'Join thousands of users who are making money with our platform. Simple, fast, and secure.',
                'get_started': 'Get Started - It\'s Free',
                'feature1_title': 'Easy Earnings',
                'feature1_desc': 'Complete simple tasks and start earning money immediately.',
                'feature2_title': 'Referral Program',
                'feature2_desc': 'Earn 20% of your referrals\' earnings for life.',
                'feature3_title': 'Secure Payments',
                'feature3_desc': 'Fast and secure withdrawals to your Indian bank account or UPI.',
                'quick_actions': 'Quick Actions',
                'earn_money': 'Earn Money',
                'refer_friends': 'Refer Friends',
                'transaction_history': 'Transaction History',
                'settings': 'Settings',
                'recent_activity': 'Recent Activity',
                'view_all': 'View All',
                'referral_bonus': 'Referral Bonus',
                'today_1045am': 'Today, 10:45 AM',
                'task_completion': 'Task Completion',
                'yesterday_330pm': 'Yesterday, 3:30 PM',
                'withdrawal': 'Withdrawal',
                'may_12_2023': 'May 12, 2023',
                'referral_program': 'Referral Program',
                'earn_20_commission': 'Earn 20% commission',
                'referral_desc': 'on your referrals\' earnings for life!',
                'copy': 'Copy',
                'withdraw_funds': 'Withdraw Funds',
                'min_withdraw_info': 'Minimum withdrawal amount is ₹200. Processing time is 3-5 business days.',
                'amount': 'Am
