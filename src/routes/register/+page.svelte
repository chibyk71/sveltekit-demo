<svelte:head>
    <title>Website||Register</title>
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
                        <h1>Welcome friend!</h1>
                    </div>
                </div>
            </div>
            <div class="col-xl-6 col-lg-7 col-md-10 col-12 m-auto">
                <div class="login-form">
                    <div>
                        <div class="login-title">
                            <h2>Register</h2>
                        </div>
                        <div class="login-discription">
                            <h3>Hello Everyone</h3>
                            <h4>Welcome to Friendbook, create your account below to start usinf friendbook.</h4>
                        </div>
                        <div class="form-sec">
                            <div>
                                <form class="theme-form">
                                    <div class="form-group">
                                        <label for="name">Full Name</label>
                                        <input type="text" class="form-control" id="name" placeholder="Your Name">
                                        <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-user input-icon iw-20 ih-20"><path d="M20 21v-2a4 4 0 0 0-4-4H8a4 4 0 0 0-4 4v2"></path><circle cx="12" cy="7" r="4"></circle></svg>
                                    </div>
                                    <div class="form-group">
                                        <label for="exampleInputEmail1">Email address</label>
                                        <input type="email" class="form-control" id="exampleInputEmail1" placeholder="Enter email">
                                        <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-mail input-icon iw-20 ih-20"><path d="M4 4h16c1.1 0 2 .9 2 2v12c0 1.1-.9 2-2 2H4c-1.1 0-2-.9-2-2V6c0-1.1.9-2 2-2z"></path><polyline points="22,6 12,13 2,6"></polyline></svg>
                                    </div>
                                    <div class="form-group">
                                        <label for="exampleInputPassword1">Password</label>
                                        <input type="password" class="form-control" id="exampleInputPassword1" placeholder="Password">
                                        <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-eye input-icon iw-20 ih-20"><path d="M1 12s4-8 11-8 11 8 11 8-4 8-11 8-11-8-11-8z"></path><circle cx="12" cy="12" r="3"></circle></svg>
                                        <!-- <i class="input-icon iw-20 ih-20" data-feather="eye-off"></i> -->
                                    </div>
                                    <div class="bottom-sec">
                                        <div class="form-check checkbox_animated">
                                            <input type="checkbox" class="form-check-input" id="exampleCheck1">
                                            <label class="form-check-label" for="exampleCheck1">remember me</label>
                                        </div>
                                        <a href="#" class="ms-auto">forget password?</a>
                                    </div>
                                    <div class="btn-section">
                                        <a href="#" class="btn btn-solid btn-lg">sign up</a>
                                        <a href="login" class="btn btn-solid btn-lg ms-auto">login</a>
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
                    Friendbook is a website which allows users, who sign-up for free profiles, to connect with
                    friends, work colleagues or people they don't know, online.
                </p>
            </div>
        </div>
    </div>
</section>