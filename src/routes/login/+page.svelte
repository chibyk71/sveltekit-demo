<script>
    import stNm from "$lib/constant.js";
</script>

<svelte:head>
    <title>{stNm}||Login</title>
</svelte:head>

<section class="login-section">
    <div class="header-section">
        <div class="logo-sec">
            <a href="index.html">
                <img src="images/icon/logo.png" alt="logo" class="img-fluid blur-up lazyloaded">
            </a>
        </div>
        <div class="right-links">
            <ul>
                <li>
                    <a href="#">
                        about
                    </a>
                </li>
                <li>
                    <a href="#">
                        upgrade
                    </a>
                </li>
            </ul>
        </div>
    </div>
    <div class="container">
        <div class="row">
            <div class="col-xl-6 col-lg-5 d-none d-lg-block">
                <div class="login-welcome">
                    <div>
                        <img src="images/login/charcter.png" class="img-fluid blur-up lazyloaded" alt="charcter">
                        <h1>Welcome Back!</h1>
                    </div>
                </div>
            </div>
            <div class="col-xl-6 col-lg-7 col-md-10 col-12 m-auto">
                <div class="login-form">
                    <div>
                        <div class="login-title">
                            <h2>Login</h2>
                        </div>
                        <div class="login-discription">
                            <h3>Hello Everyone, Welcome Back</h3>
                            <h4>Welcome to Friendbook, please login to your account.
                            </h4>
                        </div>
                        <div class="form-sec">
                            <div>
                                <form class="theme-form">
                                    <div class="form-group">
                                        <label for="exampleInputEmail1">Email address</label>
                                        <input type="email" class="form-control" id="exampleInputEmail1" placeholder="Enter email">
                                        <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-user input-icon iw-20 ih-20"><path d="M20 21v-2a4 4 0 0 0-4-4H8a4 4 0 0 0-4 4v2"></path><circle cx="12" cy="7" r="4"></circle></svg>
                                    </div>
                                    <div class="form-group">
                                        <label for="exampleInputPassword1">Password</label>
                                        <input type="password" class="form-control" id="exampleInputPassword1" placeholder="Password">
                                        <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-eye input-icon iw-20 ih-20"><path d="M1 12s4-8 11-8 11 8 11 8-4 8-11 8-11-8-11-8z"></path><circle cx="12" cy="12" r="3"></circle></svg>
                                        <!-- <i class="input-icon" data-feather="eye-off" width="20" height="20"></i> -->
                                    </div>
                                    <div class="bottom-sec">
                                        <div class="form-check checkbox_animated">
                                            <input type="checkbox" class="form-check-input" id="exampleCheck1">
                                            <label class="form-check-label" for="exampleCheck1">remember me</label>
                                        </div>
                                        <a href="#" class="ms-auto forget-password">forget
                                            password?</a>
                                    </div>
                                    <div class="btn-section">
                                        <a href="#" class="btn btn-solid btn-lg">login</a>
                                        <a href="register" class="btn btn-solid btn-lg ms-auto">sign up</a>
                                    </div>
                                </form>
                                <div class="connect-with">
                                    <h6><span>OR Connect With</span></h6>
                                    <ul class="social-links">
                                        <li class="google">
                                            <a href="#">
                                                <svg class="">
                                                    <use xlink:href="svg/icons.svg#google"></use>
                                                </svg>
                                            </a>
                                        </li>
                                        <li class="facebook">
                                            <a href="#">
                                                <svg class="">
                                                    <use xlink:href="svg/icons.svg#facebook"></use>
                                                </svg>
                                            </a>
                                        </li>
                                        <li class="twitter">
                                            <a href="#">
                                                <svg class="">
                                                    <use xlink:href="svg/icons.svg#twitter"></use>
                                                </svg>
                                            </a>
                                        </li>
                                    </ul>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
    <div class="how-work">
        <div class="media">
            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-play-circle"><circle cx="12" cy="12" r="10"></circle><polygon points="10 8 16 12 10 16 10 8"></polygon></svg>
            <div class="media-body">
                <h2>how it work?</h2>
                <p>
                    Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been.
                </p>
            </div>
        </div>
    </div>
</section>