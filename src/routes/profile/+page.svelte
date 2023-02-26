<script>
    /** @type {import('./$types').PageData} */
    // export let data;
</script>

<div class="page-center">

    <!-- profile cover start -->
    <div class="profile-cover bg-size blur-up lazyloaded" style="background-image: url(&quot;../assets/images/cover/1.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
        <img src="../assets/images/cover/1.jpg" class="img-fluid blur-up lazyload bg-img" alt="cover" style="display: none;">
        <div class="profile-box d-lg-block d-none">
            <div class="profile-content">
                <div class="image-section">
                    <div class="profile-img">
                        <div class="bg-size blur-up lazyloaded" style="background-image: url(&quot;../assets/images/user-sm/15.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                            <img src="../assets/images/user-sm/15.jpg" class="img-fluid blur-up lazyload bg-img" alt="profile" style="display: none;">
                        </div>
                        <span class="stats">
                            <img src="../assets/images/icon/verified.png" class="img-fluid blur-up lazyloaded" alt="verified">
                        </span>
                    </div>
                </div>
                <div class="profile-detail">
                    <h2>kelin jasen <span>❤</span></h2>
                    <h5>kelin.jasen156@gmail.com</h5>
                    <div class="counter-stats">
                        <ul>
                            <li>
                                <h3 class="counter-value" data-count="546">546</h3>
                                <h5>following</h5>
                            </li>
                            <li>
                                <h3 class="counter-value" data-count="26335">26335</h3>
                                <h5>likes</h5>
                            </li>
                            <li>
                                <h3 class="counter-value" data-count="6845">6845</h3>
                                <h5>followers</h5>
                            </li>
                        </ul>
                    </div>
                    <a href="javascript:void(0)" data-bs-toggle="modal" data-bs-target="#editProfile" class="btn btn-solid">edit profile</a>
                </div>
            </div>
        </div>
        <div class="setting-dropdown btn-group custom-dropdown arrow-none dropdown-sm">
            <a class="btn-white btn-cover" href="#" data-bs-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
                edit cover
            </a>
            <div class="dropdown-menu dropdown-menu-right custom-dropdown" style="">
                <ul>
                    <li>
                        <a href="javascript:void(0)" data-bs-toggle="modal" data-bs-target="#choosePhoto"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-image icon-font-light iw-16 ih-16"><rect x="3" y="3" width="18" height="18" rx="2" ry="2"></rect><circle cx="8.5" cy="8.5" r="1.5"></circle><polyline points="21 15 16 10 5 21"></polyline></svg>choose
                            photo</a>
                    </li>
                    <li class="choose-file">
                        <a href=""><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-upload icon-font-light iw-16 ih-16"><path d="M21 15v4a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2v-4"></path><polyline points="17 8 12 3 7 8"></polyline><line x1="12" y1="3" x2="12" y2="15"></line></svg>upload
                            photo</a>
                        <input type="file">
                    </li>
                    <li>
                        <a href=""><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-maximize icon-font-light iw-16 ih-16"><path d="M8 3H5a2 2 0 0 0-2 2v3m18 0V5a2 2 0 0 0-2-2h-3m0 18h3a2 2 0 0 0 2-2v-3M3 16v3a2 2 0 0 0 2 2h3"></path></svg>set
                            position</a>
                    </li>
                    <li>
                        <a href=""><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-trash-2 icon-font-light iw-16 ih-16"><polyline points="3 6 5 6 21 6"></polyline><path d="M19 6v14a2 2 0 0 1-2 2H7a2 2 0 0 1-2-2V6m3 0V4a2 2 0 0 1 2-2h4a2 2 0 0 1 2 2v2"></path><line x1="10" y1="11" x2="10" y2="17"></line><line x1="14" y1="11" x2="14" y2="17"></line></svg>remove
                            photo</a>
                    </li>
                </ul>
            </div>
        </div>
    </div>
    <div class="d-lg-none d-block">
        <div class="profile-box">
            <div class="profile-content">
                <div class="image-section">
                    <div class="profile-img">
                        <div class="bg-size blur-up lazyloaded" style="background-image: url(&quot;../assets/images/user-sm/15.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                            <img src="../assets/images/user-sm/15.jpg" class="img-fluid blur-up lazyload bg-img" alt="profile" style="display: none;">
                        </div>
                        <span class="stats">
                            <img src="../assets/images/icon/verified.png" class="img-fluid blur-up lazyloaded" alt="verified">
                        </span>
                    </div>
                </div>
                <div class="profile-detail">
                    <h2>kelin jasen <span>❤</span></h2>
                    <h5>kelin.jasen156@gmail.com</h5>
                    <div class="counter-stats">
                        <ul id="counter">
                            <li>
                                <h3 class="counter-value" data-count="546">546</h3>
                                <h5>following</h5>
                            </li>
                            <li>
                                <h3 class="counter-value" data-count="26335">26335</h3>
                                <h5>likes</h5>
                            </li>
                            <li>
                                <h3 class="counter-value" data-count="6845">6845</h3>
                                <h5>followers</h5>
                            </li>
                        </ul>
                    </div>
                    <a href="javascript:void(0)" data-bs-toggle="modal" data-bs-target="#editProfile" class="btn btn-solid">edit profile</a>
                </div>
            </div>
        </div>
    </div>
    <!-- profile cover end -->

    <!-- profile menu start -->
    <div class="profile-menu section-t-space">
        <ul>
            <li class="active">
                <a href="profile.html">
                    <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-clock iw-14 ih-14"><circle cx="12" cy="12" r="10"></circle><polyline points="12 6 12 12 16 14"></polyline></svg>
                    <h6>timeline</h6>
                </a>
            </li>
            <li>
                <a href="profile-about.html">
                    <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-info iw-14 ih-14"><circle cx="12" cy="12" r="10"></circle><line x1="12" y1="16" x2="12" y2="12"></line><line x1="12" y1="8" x2="12.01" y2="8"></line></svg>
                    <h6>about</h6>
                </a>
            </li>
            <li>
                <a href="profile-friends.html">
                    <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-users iw-14 ih-14"><path d="M17 21v-2a4 4 0 0 0-4-4H5a4 4 0 0 0-4 4v2"></path><circle cx="9" cy="7" r="4"></circle><path d="M23 21v-2a4 4 0 0 0-3-3.87"></path><path d="M16 3.13a4 4 0 0 1 0 7.75"></path></svg>
                    <h6>friends</h6>
                </a>
            </li>
            <li>
                <a href="profile-gallery.html">
                    <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-image iw-14 ih-14"><rect x="3" y="3" width="18" height="18" rx="2" ry="2"></rect><circle cx="8.5" cy="8.5" r="1.5"></circle><polyline points="21 15 16 10 5 21"></polyline></svg>
                    <h6>photos</h6>
                </a>
            </li>
            <li class="d-xl-none d-inline-block">
                <a href="profile-activityfeed.html">
                    <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-list iw-14 ih-14"><line x1="8" y1="6" x2="21" y2="6"></line><line x1="8" y1="12" x2="21" y2="12"></line><line x1="8" y1="18" x2="21" y2="18"></line><line x1="3" y1="6" x2="3.01" y2="6"></line><line x1="3" y1="12" x2="3.01" y2="12"></line><line x1="3" y1="18" x2="3.01" y2="18"></line></svg>
                    <h6>acitivity feed</h6>
                </a>
            </li>
        </ul>
        <ul class="right-menu d-xl-flex d-none">
            <li>
                <div class="search-bar input-style icon-left search-inmenu">
                    <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-search iw-16 ih-16 icon icon-theme"><circle cx="11" cy="11" r="8"></circle><line x1="21" y1="21" x2="16.65" y2="16.65"></line></svg>
                    <input type="text" class="form-control" placeholder="search here...">
                </div>
            </li>
            <li class="active">
                <a href="profile-activityfeed.html">
                    <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-list iw-14 ih-14"><line x1="8" y1="6" x2="21" y2="6"></line><line x1="8" y1="12" x2="21" y2="12"></line><line x1="8" y1="18" x2="21" y2="18"></line><line x1="3" y1="6" x2="3.01" y2="6"></line><line x1="3" y1="12" x2="3.01" y2="12"></line><line x1="3" y1="18" x2="3.01" y2="18"></line></svg>
                    <h6>acitivity feed</h6>
                </a>
            </li>
        </ul>
    </div>
    <!-- profile menu end -->

    <div class="container-fluid section-t-space px-0 layout-default">
        <div class="page-content">
            <div class="content-left">
                <!-- profile box -->
                <div class="profile-about">
                    <div class="card-title">
                        <h3>about</h3>
                        <h5>intro my self</h5>
                        <div class="settings">
                            <div class="setting-btn">
                                <a href="#" data-bs-toggle="modal" data-bs-target="#editProfile">
                                    <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-edit-2 icon icon-dark stroke-width-3 iw-11 ih-11"><path d="M17 3a2.828 2.828 0 1 1 4 4L7.5 20.5 2 22l1.5-5.5L17 3z"></path></svg>
                                </a>
                            </div>
                        </div>
                    </div>
                    <div class="about-content">
                        <ul>
                            <li>
                                <div class="icon">
                                    <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-briefcase iw-18 ih-18"><rect x="2" y="7" width="20" height="14" rx="2" ry="2"></rect><path d="M16 21V5a2 2 0 0 0-2-2h-4a2 2 0 0 0-2 2v16"></path></svg>
                                </div>
                                <div class="details">
                                    <h5>UX desginer at google</h5>
                                    <h6>banglore - 2019</h6>
                                </div>
                            </li>
                            <li>
                                <div class="icon">
                                    <svg>
                                        <use class="fill-color" xlink:href="../assets/svg/icons.svg#degree">
                                        </use>
                                    </svg>
                                </div>
                                <div class="details">
                                    <h5>studied computer science</h5>
                                    <h6>at london univercity - 2015</h6>
                                </div>
                            </li>
                            <li>
                                <div class="icon">
                                    <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-heart iw-18 ih-18"><path d="M20.84 4.61a5.5 5.5 0 0 0-7.78 0L12 5.67l-1.06-1.06a5.5 5.5 0 0 0-7.78 7.78l1.06 1.06L12 21.23l7.78-7.78 1.06-1.06a5.5 5.5 0 0 0 0-7.78z"></path></svg>
                                </div>
                                <div class="details">
                                    <h5>relationship status</h5>
                                    <h6>single</h6>
                                </div>
                            </li>
                            <li>
                                <div class="icon">
                                    <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-map-pin iw-18 ih-18"><path d="M21 10c0 7-9 13-9 13s-9-6-9-13a9 9 0 0 1 18 0z"></path><circle cx="12" cy="10" r="3"></circle></svg>
                                </div>
                                <div class="details">
                                    <h5>lived in london</h5>
                                    <h6>last 5 year</h6>
                                </div>
                            </li>
                            <li>
                                <div class="icon">
                                    <svg>
                                        <use class="fill-color" xlink:href="../assets/svg/icons.svg#blood-drop">
                                        </use>
                                    </svg>
                                </div>
                                <div class="details">
                                    <h5>blood group</h5>
                                    <h6>A+ positive</h6>
                                </div>
                            </li>
                        </ul>
                    </div>
                    <div class="about-footer">
                        <ul>
                            <li class="fb">
                                <a href="#">
                                    <svg>
                                        <use xlink:href="../assets/svg/icons.svg#facebook"></use>
                                    </svg>
                                </a>
                            </li>
                            <li class="tw">
                                <a href="#">
                                    <svg>
                                        <use xlink:href="../assets/svg/icons.svg#twitter"></use>
                                    </svg>
                                </a>
                            </li>
                            <li class="wa">
                                <a href="#">
                                    <svg>
                                        <use xlink:href="../assets/svg/icons.svg#whatsapp"></use>
                                    </svg>
                                </a>
                            </li>
                        </ul>
                    </div>
                </div>
                <!-- suggestion box -->
                <div class="suggestion-box section-t-space d-xl-block d-none">
                    <div class="card-title">
                        <h3>friend suggestion</h3>
                        <div class="settings">
                            <div class="setting-btn">
                                <a href="#" class="d-flex">
                                    <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-rotate-cw icon icon-theme stroke-width-3 iw-11 ih-11"><polyline points="23 4 23 10 17 10"></polyline><path d="M20.49 15a9 9 0 1 1-2.12-9.36L23 10"></path></svg>
                                </a>
                            </div>
                            <div class="setting-btn setting-dropdown ms-2">
                                <div class="btn-group custom-dropdown arrow-none dropdown-sm">
                                    <a href="#" class="d-flex" data-bs-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
                                        <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-sun icon icon-theme stroke-width-3 iw-11 ih-11"><circle cx="12" cy="12" r="5"></circle><line x1="12" y1="1" x2="12" y2="3"></line><line x1="12" y1="21" x2="12" y2="23"></line><line x1="4.22" y1="4.22" x2="5.64" y2="5.64"></line><line x1="18.36" y1="18.36" x2="19.78" y2="19.78"></line><line x1="1" y1="12" x2="3" y2="12"></line><line x1="21" y1="12" x2="23" y2="12"></line><line x1="4.22" y1="19.78" x2="5.64" y2="18.36"></line><line x1="18.36" y1="5.64" x2="19.78" y2="4.22"></line></svg>
                                    </a>
                                    <div class="dropdown-menu dropdown-menu-right custom-dropdown">
                                        <ul>
                                            <li>
                                                <a href=""><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-user icon-font-light iw-16 ih-16"><path d="M20 21v-2a4 4 0 0 0-4-4H8a4 4 0 0 0-4 4v2"></path><circle cx="12" cy="7" r="4"></circle></svg>see all</a>
                                            </li>
                                            <li>
                                                <a href=""><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-search icon-font-light iw-16 ih-16"><circle cx="11" cy="11" r="8"></circle><line x1="21" y1="21" x2="16.65" y2="16.65"></line></svg>find friends</a>
                                            </li>
                                            <li>
                                                <a href=""><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-settings icon-font-light iw-16 ih-16"><circle cx="12" cy="12" r="3"></circle><path d="M19.4 15a1.65 1.65 0 0 0 .33 1.82l.06.06a2 2 0 0 1 0 2.83 2 2 0 0 1-2.83 0l-.06-.06a1.65 1.65 0 0 0-1.82-.33 1.65 1.65 0 0 0-1 1.51V21a2 2 0 0 1-2 2 2 2 0 0 1-2-2v-.09A1.65 1.65 0 0 0 9 19.4a1.65 1.65 0 0 0-1.82.33l-.06.06a2 2 0 0 1-2.83 0 2 2 0 0 1 0-2.83l.06-.06a1.65 1.65 0 0 0 .33-1.82 1.65 1.65 0 0 0-1.51-1H3a2 2 0 0 1-2-2 2 2 0 0 1 2-2h.09A1.65 1.65 0 0 0 4.6 9a1.65 1.65 0 0 0-.33-1.82l-.06-.06a2 2 0 0 1 0-2.83 2 2 0 0 1 2.83 0l.06.06a1.65 1.65 0 0 0 1.82.33H9a1.65 1.65 0 0 0 1-1.51V3a2 2 0 0 1 2-2 2 2 0 0 1 2 2v.09a1.65 1.65 0 0 0 1 1.51 1.65 1.65 0 0 0 1.82-.33l.06-.06a2 2 0 0 1 2.83 0 2 2 0 0 1 0 2.83l-.06.06a1.65 1.65 0 0 0-.33 1.82V9a1.65 1.65 0 0 0 1.51 1H21a2 2 0 0 1 2 2 2 2 0 0 1-2 2h-.09a1.65 1.65 0 0 0-1.51 1z"></path></svg>settings</a>
                                            </li>
                                        </ul>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                    <div class="suggestion-content ratio_115">
                        <div class="slide-2 no-arrow default-space slick-initialized slick-slider"><button class="slick-prev slick-arrow" aria-label="Previous" type="button" aria-disabled="false" style="display: inline-block;">Previous</button><div class="slick-list draggable"><div class="slick-track" style="opacity: 1; width: 405px; transform: translate3d(-135px, 0px, 0px);"><div class="slick-slide" data-slick-index="0" aria-hidden="true" tabindex="-1" style="width: 135px;"><div><div style="width: 100%; display: inline-block;">
                                <div class="story-box">
                                    <div class="adaptive-overlay pink-overlay"></div>
                                    <div class="story-bg bg-size" style="background-image: url(&quot;../assets/images/story/2.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                                        <img src="../assets/images/story/2.jpg" class="img-fluid bg-img" data-adaptive-background="1" alt="" style="display: none;">
                                    </div>
                                    <div class="story-content">
                                        <h6>josephin water</h6>
                                        <span>active now</span>
                                    </div>
                                </div>
                            </div></div></div><div class="slick-slide slick-current slick-active" data-slick-index="1" aria-hidden="false" style="width: 135px;"><div><div style="width: 100%; display: inline-block;">
                                <div class="story-box">
                                    <div class="adaptive-overlay blue-overlay"></div>
                                    <div class="story-bg bg-size" style="background-image: url(&quot;../assets/images/story/7.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                                        <img src="../assets/images/story/7.jpg" class="img-fluid bg-img" data-adaptive-background="1" alt="" style="display: none;">
                                    </div>
                                    <div class="story-content">
                                        <h6>josephin water</h6>
                                        <span>active now</span>
                                    </div>
                                </div>
                            </div></div></div><div class="slick-slide slick-active" data-slick-index="2" aria-hidden="false" style="width: 135px;"><div><div style="width: 100%; display: inline-block;">
                                <div class="story-box">
                                    <div class="adaptive-overlay skin-overlay"></div>
                                    <div class="story-bg bg-size" style="background-image: url(&quot;../assets/images/story/1.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                                        <img src="../assets/images/story/1.jpg" class="img-fluid bg-img" data-adaptive-background="1" alt="" style="display: none;">
                                    </div>
                                    <div class="story-content">
                                        <h6>josephin water</h6>
                                        <span>active now</span>
                                    </div>
                                </div>
                            </div></div></div></div></div><button class="slick-next slick-arrow slick-disabled" aria-label="Next" type="button" style="display: inline-block;" aria-disabled="true">Next</button></div>
                    </div>
                </div>
                <div class="sticky-top d-xl-block d-none">
                    <!-- like page -->
                    <div class="page-list section-t-space">
                        <div class="card-title">
                            <h3>liked pages</h3>
                            <h5>18 pages</h5>
                            <div class="settings">
                                <div class="setting-btn">
                                    <a href="#" class="d-flex">
                                        <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-rotate-cw icon icon-dark stroke-width-3 iw-11 ih-11"><polyline points="23 4 23 10 17 10"></polyline><path d="M20.49 15a9 9 0 1 1-2.12-9.36L23 10"></path></svg>
                                    </a>
                                </div>
                                <div class="setting-btn ms-2 setting-dropdown">
                                    <div class=" btn-group custom-dropdown arrow-none dropdown-sm">
                                        <a href="#" data-bs-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
                                            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-sun icon-dark stroke-width-3 icon iw-11 ih-11"><circle cx="12" cy="12" r="5"></circle><line x1="12" y1="1" x2="12" y2="3"></line><line x1="12" y1="21" x2="12" y2="23"></line><line x1="4.22" y1="4.22" x2="5.64" y2="5.64"></line><line x1="18.36" y1="18.36" x2="19.78" y2="19.78"></line><line x1="1" y1="12" x2="3" y2="12"></line><line x1="21" y1="12" x2="23" y2="12"></line><line x1="4.22" y1="19.78" x2="5.64" y2="18.36"></line><line x1="18.36" y1="5.64" x2="19.78" y2="4.22"></line></svg>
                                        </a>
                                        <div class="dropdown-menu dropdown-menu-right custom-dropdown">
                                            <ul>
                                                <li>
                                                    <a href=""><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-edit icon-font-light iw-16 ih-16"><path d="M11 4H4a2 2 0 0 0-2 2v14a2 2 0 0 0 2 2h14a2 2 0 0 0 2-2v-7"></path><path d="M18.5 2.5a2.121 2.121 0 0 1 3 3L12 15l-4 1 1-4 9.5-9.5z"></path></svg>see all</a>
                                                </li>
                                                <li>
                                                    <a href=""><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-search icon-font-light iw-16 ih-16"><circle cx="11" cy="11" r="8"></circle><line x1="21" y1="21" x2="16.65" y2="16.65"></line></svg>find
                                                        page</a>
                                                </li>
                                                <li>
                                                    <a href=""><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-settings icon-font-light iw-16 ih-16"><circle cx="12" cy="12" r="3"></circle><path d="M19.4 15a1.65 1.65 0 0 0 .33 1.82l.06.06a2 2 0 0 1 0 2.83 2 2 0 0 1-2.83 0l-.06-.06a1.65 1.65 0 0 0-1.82-.33 1.65 1.65 0 0 0-1 1.51V21a2 2 0 0 1-2 2 2 2 0 0 1-2-2v-.09A1.65 1.65 0 0 0 9 19.4a1.65 1.65 0 0 0-1.82.33l-.06.06a2 2 0 0 1-2.83 0 2 2 0 0 1 0-2.83l.06-.06a1.65 1.65 0 0 0 .33-1.82 1.65 1.65 0 0 0-1.51-1H3a2 2 0 0 1-2-2 2 2 0 0 1 2-2h.09A1.65 1.65 0 0 0 4.6 9a1.65 1.65 0 0 0-.33-1.82l-.06-.06a2 2 0 0 1 0-2.83 2 2 0 0 1 2.83 0l.06.06a1.65 1.65 0 0 0 1.82.33H9a1.65 1.65 0 0 0 1-1.51V3a2 2 0 0 1 2-2 2 2 0 0 1 2 2v.09a1.65 1.65 0 0 0 1 1.51 1.65 1.65 0 0 0 1.82-.33l.06-.06a2 2 0 0 1 2.83 0 2 2 0 0 1 0 2.83l-.06.06a1.65 1.65 0 0 0-.33 1.82V9a1.65 1.65 0 0 0 1.51 1H21a2 2 0 0 1 2 2 2 2 0 0 1-2 2h-.09a1.65 1.65 0 0 0-1.51 1z"></path></svg>settings</a>
                                                </li>
                                            </ul>
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                        <div class="list-content">
                            <ul>
                                <li>
                                    <div class="media">
                                        <div class="img-part bg-size blur-up lazyloaded" style="background-image: url(&quot;../assets/images/pages-logo/1.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                                            <img src="../assets/images/pages-logo/1.jpg" class="img-fluid blur-up lazyload bg-img" alt="" style="display: none;">
                                        </div>
                                        <div class="media-body">
                                            <h4>chrimson agency</h4>
                                            <h6>clothing store
                                                <span><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-user icon-font-color iw-13 ih-13"><path d="M20 21v-2a4 4 0 0 0-4-4H8a4 4 0 0 0-4 4v2"></path><circle cx="12" cy="7" r="4"></circle></svg>15k</span>
                                            </h6>
                                        </div>
                                    </div>
                                    <div class="favourite-btn active">
                                        <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-star icon-dark iw-14 ih-14"><polygon points="12 2 15.09 8.26 22 9.27 17 14.14 18.18 21.02 12 17.77 5.82 21.02 7 14.14 2 9.27 8.91 8.26 12 2"></polygon></svg>
                                    </div>
                                </li>
                                <li>
                                    <div class="media">
                                        <div class="img-part bg-size blur-up lazyload" style="background-image: url(&quot;../assets/images/pages-logo/2.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                                            <img src="../assets/images/pages-logo/2.jpg" class="img-fluid blur-up lazyload bg-img" alt="" style="display: none;">
                                        </div>
                                        <div class="media-body">
                                            <h4>Digital Pixel</h4>
                                            <h6>software company
                                                <span><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-user icon-font-color iw-13 ih-13"><path d="M20 21v-2a4 4 0 0 0-4-4H8a4 4 0 0 0-4 4v2"></path><circle cx="12" cy="7" r="4"></circle></svg>158k</span>
                                            </h6>
                                        </div>
                                    </div>
                                    <div class="favourite-btn">
                                        <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-star icon-dark iw-14 ih-14"><polygon points="12 2 15.09 8.26 22 9.27 17 14.14 18.18 21.02 12 17.77 5.82 21.02 7 14.14 2 9.27 8.91 8.26 12 2"></polygon></svg>
                                    </div>
                                </li>
                                <li>
                                    <div class="media">
                                        <div class="img-part bg-size blur-up lazyload" style="background-image: url(&quot;../assets/images/pages-logo/3.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                                            <img src="../assets/images/pages-logo/3.jpg" class="img-fluid blur-up lazyload bg-img" alt="" style="display: none;">
                                        </div>
                                        <div class="media-body">
                                            <h4>the angle bar</h4>
                                            <h6>disco bar
                                                <span><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-user icon-font-color iw-13 ih-13"><path d="M20 21v-2a4 4 0 0 0-4-4H8a4 4 0 0 0-4 4v2"></path><circle cx="12" cy="7" r="4"></circle></svg>8k</span>
                                            </h6>
                                        </div>
                                    </div>
                                    <div class="favourite-btn active">
                                        <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-star icon-dark iw-14 ih-14"><polygon points="12 2 15.09 8.26 22 9.27 17 14.14 18.18 21.02 12 17.77 5.82 21.02 7 14.14 2 9.27 8.91 8.26 12 2"></polygon></svg>
                                    </div>
                                </li>
                                <li>
                                    <div class="media">
                                        <div class="img-part bg-size blur-up lazyload" style="background-image: url(&quot;../assets/images/pages-logo/4.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                                            <img src="../assets/images/pages-logo/4.jpg" class="img-fluid blur-up lazyload bg-img" alt="" style="display: none;">
                                        </div>
                                        <div class="media-body">
                                            <h4>fivestar food</h4>
                                            <h6>restaurant
                                                <span><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-user icon-font-color iw-13 ih-13"><path d="M20 21v-2a4 4 0 0 0-4-4H8a4 4 0 0 0-4 4v2"></path><circle cx="12" cy="7" r="4"></circle></svg>186k</span>
                                            </h6>
                                        </div>
                                    </div>
                                    <div class="favourite-btn">
                                        <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-star icon-dark iw-14 ih-14"><polygon points="12 2 15.09 8.26 22 9.27 17 14.14 18.18 21.02 12 17.77 5.82 21.02 7 14.14 2 9.27 8.91 8.26 12 2"></polygon></svg>
                                    </div>
                                </li>
                                <li>
                                    <div class="media">
                                        <div class="img-part bg-size blur-up lazyload" style="background-image: url(&quot;../assets/images/pages-logo/5.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                                            <img src="../assets/images/pages-logo/5.jpg" class="img-fluid blur-up lazyload bg-img" alt="" style="display: none;">
                                        </div>
                                        <div class="media-body">
                                            <h4>royal watch</h4>
                                            <h6>watch shop
                                                <span><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-user icon-font-color iw-13 ih-13"><path d="M20 21v-2a4 4 0 0 0-4-4H8a4 4 0 0 0-4 4v2"></path><circle cx="12" cy="7" r="4"></circle></svg>65k</span>
                                            </h6>
                                        </div>
                                    </div>
                                    <div class="favourite-btn">
                                        <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-star icon-dark iw-14 ih-14"><polygon points="12 2 15.09 8.26 22 9.27 17 14.14 18.18 21.02 12 17.77 5.82 21.02 7 14.14 2 9.27 8.91 8.26 12 2"></polygon></svg>
                                    </div>
                                </li>
                            </ul>
                        </div>
                    </div>
                </div>
            </div>
            <div class="content-center">
                <!-- create post -->
                <div class="create-post">
                    <div class="static-section">
                        <div class="card-title">
                            <h3>create post</h3>
                            <ul class="create-option">
                                <li class="options">
                                    <div class="setting-dropdown">
                                        <div class="btn-group custom-dropdown arrow-none dropdown-sm">
                                            <h5 data-bs-toggle="dropdown" aria-haspopup="true" aria-expanded="false">public <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-chevron-down iw-14"><polyline points="6 9 12 15 18 9"></polyline></svg></h5>
                                            <div class="dropdown-menu dropdown-menu-right custom-dropdown">
                                                <ul>
                                                    <li>
                                                        <a href=""><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-globe icon-font-light iw-16 ih-16"><circle cx="12" cy="12" r="10"></circle><line x1="2" y1="12" x2="22" y2="12"></line><path d="M12 2a15.3 15.3 0 0 1 4 10 15.3 15.3 0 0 1-4 10 15.3 15.3 0 0 1-4-10 15.3 15.3 0 0 1 4-10z"></path></svg>public</a>
                                                    </li>
                                                    <li>
                                                        <a href=""><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-users icon-font-light iw-16 ih-16"><path d="M17 21v-2a4 4 0 0 0-4-4H5a4 4 0 0 0-4 4v2"></path><circle cx="9" cy="7" r="4"></circle><path d="M23 21v-2a4 4 0 0 0-3-3.87"></path><path d="M16 3.13a4 4 0 0 1 0 7.75"></path></svg>friends</a>
                                                    </li>
                                                    <li>
                                                        <a href=""><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-user icon-font-light iw-16 ih-16"><path d="M20 21v-2a4 4 0 0 0-4-4H8a4 4 0 0 0-4 4v2"></path><circle cx="12" cy="7" r="4"></circle></svg>friends
                                                            except</a>
                                                    </li>
                                                    <li>
                                                        <a href=""><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-user icon-font-light iw-16 ih-16"><path d="M20 21v-2a4 4 0 0 0-4-4H8a4 4 0 0 0-4 4v2"></path><circle cx="12" cy="7" r="4"></circle></svg>specific
                                                            friends</a>
                                                    </li>
                                                    <li>
                                                        <a href=""><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-lock icon-font-light iw-16 ih-16"><rect x="3" y="11" width="18" height="11" rx="2" ry="2"></rect><path d="M7 11V7a5 5 0 0 1 10 0v4"></path></svg>only me</a>
                                                    </li>
                                                </ul>
                                            </div>
                                        </div>
                                    </div>
                                </li>
                                <li>
                                    <h5><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-video iw-15"><polygon points="23 7 16 12 23 17 23 7"></polygon><rect x="1" y="5" width="15" height="14" rx="2" ry="2"></rect></svg>go live</h5>
                                </li>
                            </ul>
                            <div class="settings">
                                <div class="setting-btn ms-2 setting-dropdown no-bg">
                                    <div class="btn-group custom-dropdown arrow-none dropdown-sm">
                                        <div role="button" data-bs-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
                                            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-more-horizontal icon icon-font-color iw-14"><circle cx="12" cy="12" r="1"></circle><circle cx="19" cy="12" r="1"></circle><circle cx="5" cy="12" r="1"></circle></svg>
                                        </div>
                                        <div class="dropdown-menu dropdown-menu-right custom-dropdown">
                                            <ul>
                                                <li>
                                                    <a href=""><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-edit icon-font-light iw-16 ih-16"><path d="M11 4H4a2 2 0 0 0-2 2v14a2 2 0 0 0 2 2h14a2 2 0 0 0 2-2v-7"></path><path d="M18.5 2.5a2.121 2.121 0 0 1 3 3L12 15l-4 1 1-4 9.5-9.5z"></path></svg>edit profile</a>
                                                </li>
                                                <li>
                                                    <a href=""><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-user icon-font-light iw-16 ih-16"><path d="M20 21v-2a4 4 0 0 0-4-4H8a4 4 0 0 0-4 4v2"></path><circle cx="12" cy="7" r="4"></circle></svg>view profile</a>
                                                </li>
                                            </ul>
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                        <div class="search-input input-style icon-right">
                            <input type="text" class="form-control enable" placeholder="write something here..">
                            <a href="#">
                                <img src="../assets/images/icon/translate.png" class="img-fluid blur-up icon lazyloaded" alt="translate">
                            </a>
                        </div>
                    </div>
                    <div class="create-bg">
                        <div class="bg-post" id="bg-post">
                            <div class="input-sec">
                                <input type="text" class="form-control enable" placeholder="write something here..">
                                <div class="close-icon">
                                    <a href="javascript:void(0)">
                                        <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-x iw-20 ih-20"><line x1="18" y1="6" x2="6" y2="18"></line><line x1="6" y1="6" x2="18" y2="18"></line></svg>
                                    </a>
                                </div>
                            </div>
                        </div>
                        <ul class="gradient-bg">
                            <li onclick="clickGradient('gr-1')" class="gr-1"></li>
                            <li onclick="clickGradient('gr-2')" class="gr-2"></li>
                            <li onclick="clickGradient('gr-3')" class="gr-3"></li>
                            <li onclick="clickGradient('gr-4')" class="gr-4"></li>
                            <li onclick="clickGradient('gr-5')" class="gr-5"></li>
                            <li onclick="clickGradient('gr-6')" class="gr-6"></li>
                            <li onclick="clickGradient('gr-7')" class="gr-7"></li>
                            <li onclick="clickGradient('gr-8')" class="gr-8"></li>
                            <li onclick="clickGradient('gr-9')" class="gr-9"></li>
                            <li onclick="clickGradient('gr-10')" class="gr-10"></li>
                            <li onclick="clickGradient('gr-11')" class="gr-11"></li>
                            <li onclick="clickGradient('gr-12')" class="gr-12"></li>
                            <li onclick="clickGradient('gr-13')" class="gr-13"></li>
                            <li onclick="clickGradient('gr-14')" class="gr-14"></li>
                            <li onclick="clickGradient('gr-15')" class="gr-15"></li>
                        </ul>
                    </div>
                    <div class="options-input" id="additional-input">
                        <a id="icon-close" href="javascript:void(0)">
                            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-x iw-15 icon-font-light icon-close"><line x1="18" y1="6" x2="6" y2="18"></line><line x1="6" y1="6" x2="18" y2="18"></line></svg>
                        </a>
                        <div class="search-input feeling-input">
                            <input type="text" class="form-control enable" list="feelings" placeholder="How Are You Feeling?">
                            <datalist id="feelings">
                                <option value="Happy">
                                </option><option value="Sad">
                                </option><option value="Angry">
                                </option><option value="Worried">
                                </option><option value="Shy">
                                </option><option value="Excited">
                                </option><option value="Surprised">
                                </option><option value="Silly">
                                </option><option value="Embarrassed">
                            </option></datalist>
                            <a href="#">
                                <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-smile iw-15 icon-left icon-font-light"><circle cx="12" cy="12" r="10"></circle><path d="M8 14s1.5 2 4 2 4-2 4-2"></path><line x1="9" y1="9" x2="9.01" y2="9"></line><line x1="15" y1="9" x2="15.01" y2="9"></line></svg>
                            </a>
                        </div>
                        <div class="search-input place-input">
                            <input type="text" class="form-control" placeholder="search for places...">
                            <a href="#">
                                <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-map-pin iw-15 icon-left icon-font-light"><path d="M21 10c0 7-9 13-9 13s-9-6-9-13a9 9 0 0 1 18 0z"></path><circle cx="12" cy="10" r="3"></circle></svg>
                            </a>
                        </div>
                        <div class="search-input friend-input">
                            <input type="text" class="form-control" list="friends" placeholder="search your friends...">
                            <datalist id="friends">
                                <option value="Paige Turner">
                                </option><option value="Bob Frapples">
                                </option><option value="Josephin water">
                                </option><option value="Petey Cruiser">
                                </option><option value="Anna Sthesia">
                                </option><option value="Paul Molive">
                                </option><option value="Anna Mull">
                            </option></datalist>
                            <a href="#">
                                <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-tag iw-15 icon-left icon-font-light"><path d="M20.59 13.41l-7.17 7.17a2 2 0 0 1-2.83 0L2 12V2h10l8.59 8.59a2 2 0 0 1 0 2.82z"></path><line x1="7" y1="7" x2="7.01" y2="7"></line></svg>
                            </a>
                        </div>
                    </div>
                    <ul class="create-btm-option">
                        <li>
                            <input class="choose-file" type="file">
                            <h5><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-camera iw-14"><path d="M23 19a2 2 0 0 1-2 2H3a2 2 0 0 1-2-2V8a2 2 0 0 1 2-2h4l2-3h6l2 3h4a2 2 0 0 1 2 2z"></path><circle cx="12" cy="13" r="4"></circle></svg>album</h5>
                        </li>
                        <li id="feeling-btn">
                            <h5><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-smile iw-15"><circle cx="12" cy="12" r="10"></circle><path d="M8 14s1.5 2 4 2 4-2 4-2"></path><line x1="9" y1="9" x2="9.01" y2="9"></line><line x1="15" y1="9" x2="15.01" y2="9"></line></svg>feelings &amp; acitivity</h5>
                        </li>
                        <li id="checkin-btn">
                            <h5><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-map-pin iw-15"><path d="M21 10c0 7-9 13-9 13s-9-6-9-13a9 9 0 0 1 18 0z"></path><circle cx="12" cy="10" r="3"></circle></svg>check in</h5>
                        </li>
                        <li id="friends-btn">
                            <h5><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-tag iw-15"><path d="M20.59 13.41l-7.17 7.17a2 2 0 0 1-2.83 0L2 12V2h10l8.59 8.59a2 2 0 0 1 0 2.82z"></path><line x1="7" y1="7" x2="7.01" y2="7"></line></svg>tag friends</h5>
                        </li>
                    </ul>
                    <div id="post-btn" class="post-btn d-none">
                        <button disabled="disabled" class="Disable">post</button>
                    </div>
                </div>
                <div class="overlay-bg"></div>
                <div class="post-panel infinite-loader-sec section-t-space">
                    <div class="post-wrapper col-grid-box" style="display: block;">
                        <div class="post-title">
                            <div class="profile">
                                <div class="media">
                                    <a class="popover-cls user-img bg-size blur-up lazyloaded" data-bs-toggle="popover" data-placement="right" data-name="sufiya eliza" data-img="../assets/images/user-sm/15.jpg" style="background-image: url(&quot;../assets/images/user-sm/15.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;" data-bs-original-title="" title="">
                                        <img src="../assets/images/user-sm/15.jpg" class="img-fluid blur-up lazyload bg-img" alt="user" style="display: none;">
                                    </a>
                                    <div class="media-body">
                                        <h5>sufiya eliza</h5>
                                        <h6>30 mins ago</h6>
                                    </div>
                                </div>
                            </div>
                            <div class="setting-btn ms-auto setting-dropdown no-bg">
                                <div class="btn-group custom-dropdown arrow-none dropdown-sm">
                                    <div role="button" data-bs-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
                                        <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-more-horizontal icon icon-font-color iw-14"><circle cx="12" cy="12" r="1"></circle><circle cx="19" cy="12" r="1"></circle><circle cx="5" cy="12" r="1"></circle></svg>
                                    </div>
                                    <div class="dropdown-menu dropdown-menu-right custom-dropdown">
                                        <ul>
                                            <li>
                                                <a href=""><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-bookmark icon-font-light iw-16 ih-16"><path d="M19 21l-7-5-7 5V5a2 2 0 0 1 2-2h10a2 2 0 0 1 2 2z"></path></svg>save post</a>
                                            </li>
                                            <li>
                                                <a href=""><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-edit icon-font-light iw-16 ih-16"><path d="M11 4H4a2 2 0 0 0-2 2v14a2 2 0 0 0 2 2h14a2 2 0 0 0 2-2v-7"></path><path d="M18.5 2.5a2.121 2.121 0 0 1 3 3L12 15l-4 1 1-4 9.5-9.5z"></path></svg>edit post</a>
                                            </li>
                                            <li>
                                                <a href=""><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-x-square icon-font-light iw-16 ih-16"><rect x="3" y="3" width="18" height="18" rx="2" ry="2"></rect><line x1="9" y1="9" x2="15" y2="15"></line><line x1="15" y1="9" x2="9" y2="15"></line></svg>hide post</a>
                                            </li>
                                        </ul>
                                    </div>
                                </div>
                            </div>
                        </div>
                        <div class="post-details">
                            <div class="img-wrapper">
                                <img src="../assets/images/post/11.jpg" class="img-fluid blur-up lazyloaded" alt="">
                                <div class="controler">
                                    <a href="#" class="play" data-bs-toggle="modal" data-bs-target="#videoPlayer">
                                        <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-play-circle iw-50 ih-50"><circle cx="12" cy="12" r="10"></circle><polygon points="10 8 16 12 10 16 10 8"></polygon></svg>
                                    </a>
                                    <div class="duration">
                                        <h6>06:20</h6>
                                    </div>
                                    <a href="#" class="volume">
                                        <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-volume-2 iw-14 ih-14"><polygon points="11 5 6 9 2 9 2 15 6 15 11 19 11 5"></polygon><path d="M19.07 4.93a10 10 0 0 1 0 14.14M15.54 8.46a5 5 0 0 1 0 7.07"></path></svg>
                                    </a>
                                </div>
                            </div>
                            <div class="detail-box">
                                <h3>Today Our Three Cute Puppy Dog Birthday !!!!</h3>
                                <h5 class="tag"><span>#ourcutepuppy,</span> #puppy, #birthday, #dog</h5>
                                <p>Lorem Ipsum is simply dummy text of the printing and typesetting industry.
                                    has been the industry's standard dummy text ever since the 1500s</p>
                                <div class="bookmark favourite-btn">
                                    <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-bookmark iw-14 ih-14"><path d="M19 21l-7-5-7 5V5a2 2 0 0 1 2-2h10a2 2 0 0 1 2 2z"></path></svg>
                                </div>
                                <div class="people-likes">
                                    <ul>
                                        <li class="bg-size blur-up lazyloaded" style="background-image: url(&quot;../assets/images/user-sm/1.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                                            <img src="../assets/images/user-sm/1.jpg" class="img-fluid blur-up lazyload bg-img" alt="" style="display: none;">
                                        </li>
                                        <li class="bg-size blur-up lazyloaded" style="background-image: url(&quot;../assets/images/user-sm/2.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                                            <img src="../assets/images/user-sm/2.jpg" class="img-fluid blur-up lazyload bg-img" alt="" style="display: none;">
                                        </li>
                                        <li class="bg-size blur-up lazyloaded" style="background-image: url(&quot;../assets/images/user-sm/3.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                                            <img src="../assets/images/user-sm/3.jpg" class="img-fluid blur-up lazyload bg-img" alt="" style="display: none;">
                                        </li>
                                    </ul>
                                    <h6>+12 people react this post</h6>
                                </div>
                            </div>
                            <div class="like-panel">
                                <div class="left-emoji">
                                    <ul>
                                        <li>
                                            <img src="../assets/svg/emoji/040.svg" alt="smile">
                                        </li>
                                        <li>
                                            <img src="../assets/svg/emoji/113.svg" alt="heart">
                                        </li>
                                        <li>
                                            <img src="../assets/svg/emoji/027.svg" alt="cry">
                                        </li>
                                        <li>
                                            <img src="../assets/svg/emoji/033.svg" alt="angry">
                                        </li>
                                    </ul>
                                    <h6>+75</h6>
                                </div>
                                <div class="right-stats">
                                    <ul>
                                        <li>
                                            <h5>
                                                <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-message-square iw-16 ih-16"><path d="M21 15a2 2 0 0 1-2 2H7l-4 4V5a2 2 0 0 1 2-2h14a2 2 0 0 1 2 2z"></path></svg>
                                                <span>4565</span> comment
                                            </h5>
                                        </li>
                                        <li>
                                            <h5>
                                                <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-share iw-16 ih-16"><path d="M4 12v8a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2v-8"></path><polyline points="16 6 12 2 8 6"></polyline><line x1="12" y1="2" x2="12" y2="15"></line></svg><span>985</span>
                                                share
                                            </h5>
                                        </li>
                                    </ul>
                                </div>
                            </div>
                            <div class="post-react">
                                <ul>
                                    <li class="react-btn">
                                        <a class="react-click" href="javascript:void(0)">
                                            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-smile iw-18 ih-18"><circle cx="12" cy="12" r="10"></circle><path d="M8 14s1.5 2 4 2 4-2 4-2"></path><line x1="9" y1="9" x2="9.01" y2="9"></line><line x1="15" y1="9" x2="15.01" y2="9"></line></svg> react
                                        </a>
                                        <div class="react-box">
                                            <ul>
                                                <li data-title="smile">
                                                    <a href="javascript:void(0)">
                                                        <img src="../assets/svg/emoji/040.svg" alt="smile">
                                                    </a>
                                                </li>
                                                <li data-title="love">
                                                    <a href="javascript:void(0)">
                                                        <img src="../assets/svg/emoji/113.svg" alt="heart">
                                                    </a>
                                                </li>
                                                <li data-title="cry">
                                                    <a href="javascript:void(0)">
                                                        <img src="../assets/svg/emoji/027.svg" alt="cry">
                                                    </a>
                                                </li>
                                                <li data-title="wow">
                                                    <a href="javascript:void(0)">
                                                        <img src="../assets/svg/emoji/052.svg" alt="angry">
                                                    </a>
                                                </li>
                                                <li data-title="angry">
                                                    <a href="javascript:void(0)">
                                                        <img src="../assets/svg/emoji/039.svg" alt="angry">
                                                    </a>
                                                </li>
                                                <li data-title="haha">
                                                    <a href="javascript:void(0)">
                                                        <img src="../assets/svg/emoji/042.svg" alt="">
                                                    </a>
                                                </li>
                                            </ul>
                                        </div>
                                    </li>
                                    <li class="comment-click">
                                        <a href="javascript:void(0)">
                                            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-message-square iw-18 ih-18"><path d="M21 15a2 2 0 0 1-2 2H7l-4 4V5a2 2 0 0 1 2-2h14a2 2 0 0 1 2 2z"></path></svg> comment
                                        </a>
                                    </li>
                                    <li data-bs-target="#shareModal" data-bs-toggle="modal">
                                        <a href="javascript:void(0)">
                                            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-share iw-16 ih-16"><path d="M4 12v8a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2v-8"></path><polyline points="16 6 12 2 8 6"></polyline><line x1="12" y1="2" x2="12" y2="15"></line></svg> share
                                        </a>
                                    </li>
                                </ul>
                            </div>
                            <div class="comment-section">
                                <div class="comments d-block">
                                    <div class="ldr-comments">
                                        <ul>
                                            <li>
                                                <div class="media">
                                                    <div class="ldr-img"></div>
                                                    <div class="media-body">
                                                        <div class="contents">
                                                            <div class="ldr-content"></div>
                                                            <div class="ldr-content"></div>
                                                        </div>
                                                    </div>
                                                </div>
                                                <ul class="sub-comment">
                                                    <li>
                                                        <div class="media">
                                                            <div class="ldr-img"></div>
                                                            <div class="media-body">
                                                                <div class="contents">
                                                                    <div class="ldr-content"></div>
                                                                    <div class="ldr-content"></div>
                                                                </div>
                                                            </div>
                                                        </div>
                                                    </li>
                                                </ul>
                                            </li>
                                            <li>
                                                <div class="media">
                                                    <div class="ldr-img"></div>
                                                    <div class="media-body">
                                                        <div class="contents">
                                                            <div class="ldr-content"></div>
                                                            <div class="ldr-content"></div>
                                                        </div>
                                                    </div>
                                                </div>
                                            </li>
                                            <li>
                                                <div class="media">
                                                    <div class="ldr-img"></div>
                                                    <div class="media-body">
                                                        <div class="contents">
                                                            <div class="ldr-content"></div>
                                                            <div class="ldr-content"></div>
                                                        </div>
                                                    </div>
                                                </div>
                                            </li>
                                        </ul>
                                    </div>
                                    <div class="main-comment">
                                        <div class="media">
                                            <a href="#" class="user-img bg-size blur-up lazyloaded" style="background-image: url(&quot;../assets/images/user-sm/2.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                                                <img src="../assets/images/user-sm/2.jpg" class="img-fluid blur-up lazyload bg-img" alt="user" style="display: none;">
                                            </a>
                                            <div class="media-body">
                                                <a href="#">
                                                    <h5>Pabelo Mukrani</h5>
                                                </a>
                                                <p>Oooo Very Cute and Sweet Dog, happy birthday Cuty....
                                                    🙂
                                                </p>
                                                <ul class="comment-option">
                                                    <li><a href="#">like (5)</a></li>
                                                    <li><a href="#">reply</a></li>
                                                    <li><a href="#">translate</a></li>
                                                </ul>
                                            </div>
                                            <div class="comment-time">
                                                <h6>50 mins ago</h6>
                                            </div>
                                        </div>
                                        <div class="sub-comment">
                                            <div class="media">
                                                <a href="#" class="user-img bg-size blur-up lazyload" style="background-image: url(&quot;../assets/images/user-sm/3.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                                                    <img src="../assets/images/user-sm/3.jpg" class="img-fluid blur-up lazyload bg-img" alt="user" style="display: none;">
                                                </a>
                                                <div class="media-body">
                                                    <a href="#">
                                                        <h5>sufiya elija</h5>
                                                    </a>
                                                    <p>Thank You So Much ❤❤</p>
                                                    <ul class="comment-option">
                                                        <li><a href="#">like</a></li>
                                                        <li><a href="#">reply</a></li>
                                                        <li><a href="#">translate</a></li>
                                                    </ul>
                                                </div>
                                                <div class="comment-time">
                                                    <h6>50 mins ago</h6>
                                                </div>
                                            </div>
                                            <div class="media">
                                                <a href="#" class="user-img bg-size blur-up lazyload" style="background-image: url(&quot;../assets/images/user-sm/4.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                                                    <img src="../assets/images/user-sm/4.jpg" class="img-fluid blur-up lazyload bg-img" alt="user" style="display: none;">
                                                </a>
                                                <div class="media-body">
                                                    <a href="#">
                                                        <h5>sufiya elija</h5>
                                                    </a>
                                                    <p>Thank You So Much ❤❤</p>
                                                    <ul class="comment-option">
                                                        <li><a href="#">like</a></li>
                                                        <li><a href="#">reply</a></li>
                                                        <li><a href="#">translate</a></li>
                                                    </ul>
                                                </div>
                                                <div class="comment-time">
                                                    <h6>50 mins ago</h6>
                                                </div>
                                            </div>
                                            <a href="javascript:void(0)" class="loader">
                                                <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-rotate-cw iw-15 ih-15"><polyline points="23 4 23 10 17 10"></polyline><path d="M20.49 15a9 9 0 1 1-2.12-9.36L23 10"></path></svg> load more
                                                replies
                                            </a>
                                        </div>
                                    </div>
                                    <div class="main-comment">
                                        <div class="media">
                                            <a href="#" class="user-img bg-size blur-up lazyload" style="background-image: url(&quot;../assets/images/user-sm/2.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                                                <img src="../assets/images/user-sm/2.jpg" class="img-fluid blur-up lazyload bg-img" alt="user" style="display: none;">
                                            </a>
                                            <div class="media-body">
                                                <a href="#">
                                                    <h5>Pabelo Mukrani</h5>
                                                </a>
                                                <p>It’s party time, Sufiya..... and happy birthday cuty 🎉🎊</p>
                                                <ul class="comment-option">
                                                    <li><a href="#">like</a></li>
                                                    <li><a href="#">reply</a></li>
                                                    <li><a href="#">translate</a></li>
                                                </ul>
                                            </div>
                                            <div class="comment-time">
                                                <h6>50 mins ago</h6>
                                            </div>
                                        </div>
                                    </div>
                                </div>
                                <div class="reply">
                                    <div class="search-input input-style input-lg icon-right">
                                        <input type="text" class="form-control emojiPicker" placeholder="write a comment..">
                                        <a href="javascript:void(0)">
                                            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-smile icon icon-2 iw-14 ih-14"><circle cx="12" cy="12" r="10"></circle><path d="M8 14s1.5 2 4 2 4-2 4-2"></path><line x1="9" y1="9" x2="9.01" y2="9"></line><line x1="15" y1="9" x2="15.01" y2="9"></line></svg>
                                        </a>
                                        <a href="javascript:void(0)">
                                            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-camera icon iw-14 ih-14"><path d="M23 19a2 2 0 0 1-2 2H3a2 2 0 0 1-2-2V8a2 2 0 0 1 2-2h4l2-3h6l2 3h4a2 2 0 0 1 2 2z"></path><circle cx="12" cy="13" r="4"></circle></svg>
                                        </a>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                    <div class="post-wrapper col-grid-box section-t-space" style="display: block;">
                        <div class="post-title">
                            <div class="profile">
                                <div class="media">
                                    <a class="popover-cls user-img bg-size blur-up lazyload" data-bs-toggle="popover" data-placement="right" data-name="sufiya eliza" data-img="../assets/images/user-sm/14.jpg" style="background-image: url(&quot;../assets/images/user-sm/14.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;" data-bs-original-title="" title="">
                                        <img src="../assets/images/user-sm/14.jpg" class="img-fluid blur-up lazyload bg-img" alt="user" style="display: none;">
                                    </a>
                                    <div class="media-body">
                                        <h5>sufiya eliza</h5>
                                        <h6>30 mins ago</h6>
                                    </div>
                                </div>
                            </div>
                            <div class="setting-btn ms-auto setting-dropdown no-bg">
                                <div class="btn-group custom-dropdown arrow-none dropdown-sm">
                                    <div role="button" data-bs-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
                                        <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-more-horizontal icon icon-font-color iw-14"><circle cx="12" cy="12" r="1"></circle><circle cx="19" cy="12" r="1"></circle><circle cx="5" cy="12" r="1"></circle></svg>
                                    </div>
                                    <div class="dropdown-menu dropdown-menu-right custom-dropdown">
                                        <ul>
                                            <li>
                                                <a href=""><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-bookmark icon-font-light iw-16 ih-16"><path d="M19 21l-7-5-7 5V5a2 2 0 0 1 2-2h10a2 2 0 0 1 2 2z"></path></svg>save post</a>
                                            </li>
                                            <li>
                                                <a href=""><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-edit icon-font-light iw-16 ih-16"><path d="M11 4H4a2 2 0 0 0-2 2v14a2 2 0 0 0 2 2h14a2 2 0 0 0 2-2v-7"></path><path d="M18.5 2.5a2.121 2.121 0 0 1 3 3L12 15l-4 1 1-4 9.5-9.5z"></path></svg>edit post</a>
                                            </li>
                                            <li>
                                                <a href=""><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-x-square icon-font-light iw-16 ih-16"><rect x="3" y="3" width="18" height="18" rx="2" ry="2"></rect><line x1="9" y1="9" x2="15" y2="15"></line><line x1="15" y1="9" x2="9" y2="15"></line></svg>hide post</a>
                                            </li>
                                        </ul>
                                    </div>
                                </div>
                            </div>
                        </div>
                        <div class="post-details">
                            <div class="img-wrapper">
                                <div class="gallery-section">
                                    <div class="portfolio-section ratio_square">
                                        <div class="container-fluid p-0">
                                            <div class="row">
                                                <div class="col-8 pt-cls">
                                                    <div class="overlay">
                                                        <div class="portfolio-image">
                                                            <a href="javascript:void(0)" data-bs-toggle="modal" data-bs-target="#imageModel" class="bg-size blur-up lazyload" style="background-image: url(&quot;../assets/images/story/9.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                                                                <img src="../assets/images/story/9.jpg" alt="" class="img-fluid blur-up lazyload bg-img" style="display: none;">
                                                            </a>
                                                        </div>
                                                    </div>
                                                </div>
                                                <div class="col-4 row m-0">
                                                    <div class="col-12 pt-cls p-0">
                                                        <div class="overlay">
                                                            <div class="portfolio-image">
                                                                <a href="javascript:void(0)" data-bs-toggle="modal" data-bs-target="#imageModel" class="bg-size blur-up lazyload" style="background-image: url(&quot;../assets/images/story/10.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                                                                    <img src="../assets/images/story/10.jpg" alt="" class="img-fluid blur-up lazyload bg-img" style="display: none;">
                                                                </a>
                                                            </div>
                                                        </div>
                                                    </div>
                                                    <div class="col-12 pt-cls p-0">
                                                        <div class="overlay image-plus">
                                                            <div class="portfolio-image">
                                                                <a href="javascript:void(0)" data-bs-toggle="modal" data-bs-target="#imageModel" class="bg-size blur-up lazyload" style="background-image: url(&quot;../assets/images/story/11.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                                                                    <img src="../assets/images/story/11.jpg" alt="" class="img-fluid blur-up lazyload bg-img" style="display: none;">
                                                                    <span>+20</span>
                                                                </a>
                                                            </div>
                                                        </div>
                                                    </div>
                                                </div>
                                            </div>
                                        </div>
                                    </div>
                                </div>
                            </div>
                            <div class="detail-box">
                                <h3>Celebration new album song launched</h3>
                                <h5 class="tag"><span>#Musiccelebration,</span> #music, #party, #music</h5>
                                <p>Lorem Ipsum is simply dummy text of the printing and typesetting industry.
                                    has been the industry's standard dummy text ever since the 1500s</p>
                                <div class="bookmark favourite-btn">
                                    <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-bookmark iw-14 ih-14"><path d="M19 21l-7-5-7 5V5a2 2 0 0 1 2-2h10a2 2 0 0 1 2 2z"></path></svg>
                                </div>
                                <div class="people-likes">
                                    <ul>
                                        <li class="bg-size blur-up lazyload" style="background-image: url(&quot;../assets/images/user-sm/1.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                                            <img src="../assets/images/user-sm/1.jpg" class="img-fluid blur-up lazyload bg-img" alt="" style="display: none;">
                                        </li>
                                        <li class="bg-size blur-up lazyload" style="background-image: url(&quot;../assets/images/user-sm/2.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                                            <img src="../assets/images/user-sm/2.jpg" class="img-fluid blur-up lazyload bg-img" alt="" style="display: none;">
                                        </li>
                                        <li class="bg-size blur-up lazyload" style="background-image: url(&quot;../assets/images/user-sm/3.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                                            <img src="../assets/images/user-sm/3.jpg" class="img-fluid blur-up lazyload bg-img" alt="" style="display: none;">
                                        </li>
                                    </ul>
                                    <h6>+12 people react this post</h6>
                                </div>
                            </div>
                            <div class="like-panel">
                                <div class="left-emoji">
                                    <ul>
                                        <li>
                                            <img src="../assets/svg/emoji/040.svg" alt="smile">
                                        </li>
                                        <li>
                                            <img src="../assets/svg/emoji/113.svg" alt="heart">
                                        </li>
                                        <li>
                                            <img src="../assets/svg/emoji/027.svg" alt="cry">
                                        </li>
                                        <li>
                                            <img src="../assets/svg/emoji/033.svg" alt="angry">
                                        </li>
                                    </ul>
                                    <h6>+75</h6>
                                </div>
                                <div class="right-stats">
                                    <ul>
                                        <li>
                                            <h5>
                                                <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-message-square iw-16 ih-16"><path d="M21 15a2 2 0 0 1-2 2H7l-4 4V5a2 2 0 0 1 2-2h14a2 2 0 0 1 2 2z"></path></svg>
                                                <span>4565</span> comment
                                            </h5>
                                        </li>
                                        <li>
                                            <h5>
                                                <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-share iw-16 ih-16"><path d="M4 12v8a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2v-8"></path><polyline points="16 6 12 2 8 6"></polyline><line x1="12" y1="2" x2="12" y2="15"></line></svg><span>985</span>
                                                share
                                            </h5>
                                        </li>
                                    </ul>
                                </div>
                            </div>
                            <div class="post-react">
                                <ul>
                                    <li class="react-btn">
                                        <a class="react-click" href="javascript:void(0)">
                                            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-smile iw-18 ih-18"><circle cx="12" cy="12" r="10"></circle><path d="M8 14s1.5 2 4 2 4-2 4-2"></path><line x1="9" y1="9" x2="9.01" y2="9"></line><line x1="15" y1="9" x2="15.01" y2="9"></line></svg> react
                                        </a>
                                        <div class="react-box">
                                            <ul>
                                                <li data-title="smile">
                                                    <a href="javascript:void(0)">
                                                        <img src="../assets/svg/emoji/040.svg" alt="smile">
                                                    </a>
                                                </li>
                                                <li data-title="love">
                                                    <a href="javascript:void(0)">
                                                        <img src="../assets/svg/emoji/113.svg" alt="heart">
                                                    </a>
                                                </li>
                                                <li data-title="cry">
                                                    <a href="javascript:void(0)">
                                                        <img src="../assets/svg/emoji/027.svg" alt="cry">
                                                    </a>
                                                </li>
                                                <li data-title="wow">
                                                    <a href="javascript:void(0)">
                                                        <img src="../assets/svg/emoji/052.svg" alt="angry">
                                                    </a>
                                                </li>
                                                <li data-title="angry">
                                                    <a href="javascript:void(0)">
                                                        <img src="../assets/svg/emoji/039.svg" alt="angry">
                                                    </a>
                                                </li>
                                                <li data-title="haha">
                                                    <a href="javascript:void(0)">
                                                        <img src="../assets/svg/emoji/042.svg" alt="">
                                                    </a>
                                                </li>
                                            </ul>
                                        </div>
                                    </li>
                                    <li class="comment-click">
                                        <a href="javascript:void(0)">
                                            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-message-square iw-18 ih-18"><path d="M21 15a2 2 0 0 1-2 2H7l-4 4V5a2 2 0 0 1 2-2h14a2 2 0 0 1 2 2z"></path></svg> comment
                                        </a>
                                    </li>
                                    <li data-bs-target="#shareModal" data-bs-toggle="modal">
                                        <a href="javascript:void(0)">
                                            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-share iw-16 ih-16"><path d="M4 12v8a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2v-8"></path><polyline points="16 6 12 2 8 6"></polyline><line x1="12" y1="2" x2="12" y2="15"></line></svg> share
                                        </a>
                                    </li>
                                </ul>
                            </div>
                            <div class="comment-section">

                                <div class="comments d-none">
                                    <div class="ldr-comments">
                                        <ul>
                                            <li>
                                                <div class="media">
                                                    <div class="ldr-img"></div>
                                                    <div class="media-body">
                                                        <div class="contents">
                                                            <div class="ldr-content"></div>
                                                            <div class="ldr-content"></div>
                                                        </div>
                                                    </div>
                                                </div>
                                                <ul class="sub-comment">
                                                    <li>
                                                        <div class="media">
                                                            <div class="ldr-img"></div>
                                                            <div class="media-body">
                                                                <div class="contents">
                                                                    <div class="ldr-content"></div>
                                                                    <div class="ldr-content"></div>
                                                                </div>
                                                            </div>
                                                        </div>
                                                    </li>
                                                </ul>
                                            </li>
                                            <li>
                                                <div class="media">
                                                    <div class="ldr-img"></div>
                                                    <div class="media-body">
                                                        <div class="contents">
                                                            <div class="ldr-content"></div>
                                                            <div class="ldr-content"></div>
                                                        </div>
                                                    </div>
                                                </div>
                                            </li>
                                            <li>
                                                <div class="media">
                                                    <div class="ldr-img"></div>
                                                    <div class="media-body">
                                                        <div class="contents">
                                                            <div class="ldr-content"></div>
                                                            <div class="ldr-content"></div>
                                                        </div>
                                                    </div>
                                                </div>
                                            </li>
                                        </ul>
                                    </div>
                                    <div class="main-comment">
                                        <div class="media">
                                            <a href="#" class="user-img bg-size blur-up lazyload" style="background-image: url(&quot;../assets/images/user-sm/2.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                                                <img src="../assets/images/user-sm/2.jpg" class="img-fluid blur-up lazyload bg-img" alt="user" style="display: none;">
                                            </a>
                                            <div class="media-body">
                                                <a href="#">
                                                    <h5>Pabelo Mukrani</h5>
                                                </a>
                                                <p>Oooo Very Cute and Sweet Dog, happy birthday Cuty....
                                                    🙂
                                                </p>
                                                <ul class="comment-option">
                                                    <li><a href="#">like (5)</a></li>
                                                    <li><a href="#">reply</a></li>
                                                    <li><a href="#">translate</a></li>
                                                </ul>
                                            </div>
                                            <div class="comment-time">
                                                <h6>50 mins ago</h6>
                                            </div>
                                        </div>
                                        <div class="sub-comment">
                                            <div class="media">
                                                <a href="#" class="user-img bg-size blur-up lazyload" style="background-image: url(&quot;../assets/images/user-sm/3.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                                                    <img src="../assets/images/user-sm/3.jpg" class="img-fluid blur-up lazyload bg-img" alt="user" style="display: none;">
                                                </a>
                                                <div class="media-body">
                                                    <a href="#">
                                                        <h5>sufiya elija</h5>
                                                    </a>
                                                    <p>Thank You So Much ❤❤</p>
                                                    <ul class="comment-option">
                                                        <li><a href="#">like</a></li>
                                                        <li><a href="#">reply</a></li>
                                                        <li><a href="#">translate</a></li>
                                                    </ul>
                                                </div>
                                                <div class="comment-time">
                                                    <h6>50 mins ago</h6>
                                                </div>
                                            </div>
                                            <div class="media">
                                                <a href="#" class="user-img bg-size blur-up lazyload" style="background-image: url(&quot;../assets/images/user-sm/4.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                                                    <img src="../assets/images/user-sm/4.jpg" class="img-fluid blur-up lazyload bg-img" alt="user" style="display: none;">
                                                </a>
                                                <div class="media-body">
                                                    <a href="#">
                                                        <h5>sufiya elija</h5>
                                                    </a>
                                                    <p>Thank You So Much ❤❤</p>
                                                    <ul class="comment-option">
                                                        <li><a href="#">like</a></li>
                                                        <li><a href="#">reply</a></li>
                                                        <li><a href="#">translate</a></li>
                                                    </ul>
                                                </div>
                                                <div class="comment-time">
                                                    <h6>50 mins ago</h6>
                                                </div>
                                            </div>
                                            <a href="javascript:void(0)" class="loader">
                                                <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-rotate-cw iw-15 ih-15"><polyline points="23 4 23 10 17 10"></polyline><path d="M20.49 15a9 9 0 1 1-2.12-9.36L23 10"></path></svg> load more
                                                replies
                                            </a>
                                        </div>
                                    </div>
                                    <div class="main-comment">
                                        <div class="media">
                                            <a href="#" class="user-img bg-size blur-up lazyload" style="background-image: url(&quot;../assets/images/user-sm/2.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                                                <img src="../assets/images/user-sm/2.jpg" class="img-fluid blur-up lazyload bg-img" alt="user" style="display: none;">
                                            </a>
                                            <div class="media-body">
                                                <a href="#">
                                                    <h5>Pabelo Mukrani</h5>
                                                </a>
                                                <p>It’s party time, Sufiya..... and happy birthday cuty 🎉🎊</p>
                                                <ul class="comment-option">
                                                    <li><a href="#">like</a></li>
                                                    <li><a href="#">reply</a></li>
                                                    <li><a href="#">translate</a></li>
                                                </ul>
                                            </div>
                                            <div class="comment-time">
                                                <h6>50 mins ago</h6>
                                            </div>
                                        </div>
                                    </div>
                                </div>
                                <div class="reply">
                                    <div class="search-input input-style input-lg icon-right">
                                        <input type="text" class="form-control emojiPicker" placeholder="write a comment..">
                                        <a href="javascript:void(0)">
                                            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-smile icon icon-2 iw-14 ih-14"><circle cx="12" cy="12" r="10"></circle><path d="M8 14s1.5 2 4 2 4-2 4-2"></path><line x1="9" y1="9" x2="9.01" y2="9"></line><line x1="15" y1="9" x2="15.01" y2="9"></line></svg>
                                        </a>
                                        <a href="javascript:void(0)">
                                            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-camera icon iw-14 ih-14"><path d="M23 19a2 2 0 0 1-2 2H3a2 2 0 0 1-2-2V8a2 2 0 0 1 2-2h4l2-3h6l2 3h4a2 2 0 0 1 2 2z"></path><circle cx="12" cy="13" r="4"></circle></svg>
                                        </a>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                    <div class="post-wrapper col-grid-box section-t-space" style="display: block;">
                        <div class="post-title">
                            <div class="profile">
                                <div class="media">
                                    <a class="popover-cls user-img bg-size blur-up lazyload" data-bs-toggle="popover" data-placement="right" data-name="sufiya eliza" data-img="../assets/images/user-sm/10.jpg" style="background-image: url(&quot;../assets/images/user-sm/10.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;" data-bs-original-title="" title="">
                                        <img src="../assets/images/user-sm/10.jpg" class="img-fluid blur-up lazyload bg-img" alt="user" style="display: none;">
                                    </a>
                                    <div class="media-body">
                                        <h5>sufiya eliza</h5>
                                        <h6>30 mins ago</h6>
                                    </div>
                                </div>
                            </div>
                            <div class="setting-btn ms-auto setting-dropdown no-bg">
                                <div class="btn-group custom-dropdown arrow-none dropdown-sm">
                                    <div role="button" data-bs-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
                                        <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-more-horizontal icon icon-font-color iw-14"><circle cx="12" cy="12" r="1"></circle><circle cx="19" cy="12" r="1"></circle><circle cx="5" cy="12" r="1"></circle></svg>
                                    </div>
                                    <div class="dropdown-menu dropdown-menu-right custom-dropdown">
                                        <ul>
                                            <li>
                                                <a href=""><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-bookmark icon-font-light iw-16 ih-16"><path d="M19 21l-7-5-7 5V5a2 2 0 0 1 2-2h10a2 2 0 0 1 2 2z"></path></svg>save post</a>
                                            </li>
                                            <li>
                                                <a href=""><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-edit icon-font-light iw-16 ih-16"><path d="M11 4H4a2 2 0 0 0-2 2v14a2 2 0 0 0 2 2h14a2 2 0 0 0 2-2v-7"></path><path d="M18.5 2.5a2.121 2.121 0 0 1 3 3L12 15l-4 1 1-4 9.5-9.5z"></path></svg>edit post</a>
                                            </li>
                                            <li>
                                                <a href=""><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-x-square icon-font-light iw-16 ih-16"><rect x="3" y="3" width="18" height="18" rx="2" ry="2"></rect><line x1="9" y1="9" x2="15" y2="15"></line><line x1="15" y1="9" x2="9" y2="15"></line></svg>hide post</a>
                                            </li>
                                        </ul>
                                    </div>
                                </div>
                            </div>
                        </div>
                        <div class="post-details">
                            <div class="detail-box">
                                <h3>Celebration new album song launched</h3>
                                <h5 class="tag"><span>#Musiccelebration,</span> #music, #party, #music</h5>
                                <p>Lorem Ipsum is simply dummy text of the printing and typesetting industry.
                                    has been the industry's standard dummy text ever since the 1500s</p>
                                <div class="bookmark favourite-btn">
                                    <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-bookmark iw-14 ih-14"><path d="M19 21l-7-5-7 5V5a2 2 0 0 1 2-2h10a2 2 0 0 1 2 2z"></path></svg>
                                </div>
                                <div class="people-likes">
                                    <ul>
                                        <li class="bg-size blur-up lazyload" style="background-image: url(&quot;../assets/images/user-sm/1.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                                            <img src="../assets/images/user-sm/1.jpg" class="img-fluid blur-up lazyload bg-img" alt="" style="display: none;">
                                        </li>
                                        <li class="bg-size blur-up lazyload" style="background-image: url(&quot;../assets/images/user-sm/2.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                                            <img src="../assets/images/user-sm/2.jpg" class="img-fluid blur-up lazyload bg-img" alt="" style="display: none;">
                                        </li>
                                        <li class="bg-size blur-up lazyload" style="background-image: url(&quot;../assets/images/user-sm/3.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                                            <img src="../assets/images/user-sm/3.jpg" class="img-fluid blur-up lazyload bg-img" alt="" style="display: none;">
                                        </li>
                                    </ul>
                                    <h6>+12 people react this post</h6>
                                </div>
                            </div>
                            <div class="like-panel">
                                <div class="left-emoji">
                                    <ul>
                                        <li>
                                            <img src="../assets/svg/emoji/040.svg" alt="smile">
                                        </li>
                                        <li>
                                            <img src="../assets/svg/emoji/113.svg" alt="heart">
                                        </li>
                                        <li>
                                            <img src="../assets/svg/emoji/027.svg" alt="cry">
                                        </li>
                                        <li>
                                            <img src="../assets/svg/emoji/033.svg" alt="angry">
                                        </li>
                                    </ul>
                                    <h6>+75</h6>
                                </div>
                                <div class="right-stats">
                                    <ul>
                                        <li>
                                            <h5>
                                                <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-message-square iw-16 ih-16"><path d="M21 15a2 2 0 0 1-2 2H7l-4 4V5a2 2 0 0 1 2-2h14a2 2 0 0 1 2 2z"></path></svg>
                                                <span>4565</span> comment
                                            </h5>
                                        </li>
                                        <li>
                                            <h5>
                                                <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-share iw-16 ih-16"><path d="M4 12v8a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2v-8"></path><polyline points="16 6 12 2 8 6"></polyline><line x1="12" y1="2" x2="12" y2="15"></line></svg><span>985</span>
                                                share
                                            </h5>
                                        </li>
                                    </ul>
                                </div>
                            </div>
                            <div class="post-react">
                                <ul>
                                    <li class="react-btn">
                                        <a class="react-click" href="javascript:void(0)">
                                            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-smile iw-18 ih-18"><circle cx="12" cy="12" r="10"></circle><path d="M8 14s1.5 2 4 2 4-2 4-2"></path><line x1="9" y1="9" x2="9.01" y2="9"></line><line x1="15" y1="9" x2="15.01" y2="9"></line></svg> react
                                        </a>
                                        <div class="react-box">
                                            <ul>
                                                <li data-title="smile">
                                                    <a href="javascript:void(0)">
                                                        <img src="../assets/svg/emoji/040.svg" alt="smile">
                                                    </a>
                                                </li>
                                                <li data-title="love">
                                                    <a href="javascript:void(0)">
                                                        <img src="../assets/svg/emoji/113.svg" alt="heart">
                                                    </a>
                                                </li>
                                                <li data-title="cry">
                                                    <a href="javascript:void(0)">
                                                        <img src="../assets/svg/emoji/027.svg" alt="cry">
                                                    </a>
                                                </li>
                                                <li data-title="wow">
                                                    <a href="javascript:void(0)">
                                                        <img src="../assets/svg/emoji/052.svg" alt="angry">
                                                    </a>
                                                </li>
                                                <li data-title="angry">
                                                    <a href="javascript:void(0)">
                                                        <img src="../assets/svg/emoji/039.svg" alt="angry">
                                                    </a>
                                                </li>
                                                <li data-title="haha">
                                                    <a href="javascript:void(0)">
                                                        <img src="../assets/svg/emoji/042.svg" alt="">
                                                    </a>
                                                </li>
                                            </ul>
                                        </div>
                                    </li>
                                    <li class="comment-click">
                                        <a href="javascript:void(0)">
                                            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-message-square iw-18 ih-18"><path d="M21 15a2 2 0 0 1-2 2H7l-4 4V5a2 2 0 0 1 2-2h14a2 2 0 0 1 2 2z"></path></svg> comment
                                        </a>
                                    </li>
                                    <li data-bs-target="#shareModal" data-bs-toggle="modal">
                                        <a href="javascript:void(0)">
                                            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-share iw-16 ih-16"><path d="M4 12v8a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2v-8"></path><polyline points="16 6 12 2 8 6"></polyline><line x1="12" y1="2" x2="12" y2="15"></line></svg> share
                                        </a>
                                    </li>
                                </ul>
                            </div>
                            <div class="comment-section">
                                <div class="comments d-none">
                                    <div class="ldr-comments">
                                        <ul>
                                            <li>
                                                <div class="media">
                                                    <div class="ldr-img"></div>
                                                    <div class="media-body">
                                                        <div class="contents">
                                                            <div class="ldr-content"></div>
                                                            <div class="ldr-content"></div>
                                                        </div>
                                                    </div>
                                                </div>
                                                <ul class="sub-comment">
                                                    <li>
                                                        <div class="media">
                                                            <div class="ldr-img"></div>
                                                            <div class="media-body">
                                                                <div class="contents">
                                                                    <div class="ldr-content"></div>
                                                                    <div class="ldr-content"></div>
                                                                </div>
                                                            </div>
                                                        </div>
                                                    </li>
                                                </ul>
                                            </li>
                                            <li>
                                                <div class="media">
                                                    <div class="ldr-img"></div>
                                                    <div class="media-body">
                                                        <div class="contents">
                                                            <div class="ldr-content"></div>
                                                            <div class="ldr-content"></div>
                                                        </div>
                                                    </div>
                                                </div>
                                            </li>
                                            <li>
                                                <div class="media">
                                                    <div class="ldr-img"></div>
                                                    <div class="media-body">
                                                        <div class="contents">
                                                            <div class="ldr-content"></div>
                                                            <div class="ldr-content"></div>
                                                        </div>
                                                    </div>
                                                </div>
                                            </li>
                                        </ul>
                                    </div>
                                    <div class="main-comment">
                                        <div class="media">
                                            <a href="#" class="user-img bg-size blur-up lazyload" style="background-image: url(&quot;../assets/images/user-sm/2.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                                                <img src="../assets/images/user-sm/2.jpg" class="img-fluid blur-up lazyload bg-img" alt="user" style="display: none;">
                                            </a>
                                            <div class="media-body">
                                                <a href="#">
                                                    <h5>Pabelo Mukrani</h5>
                                                </a>
                                                <p>Oooo Very Cute and Sweet Dog, happy birthday Cuty....
                                                    🙂
                                                </p>
                                                <ul class="comment-option">
                                                    <li><a href="#">like (5)</a></li>
                                                    <li><a href="#">reply</a></li>
                                                    <li><a href="#">translate</a></li>
                                                </ul>
                                            </div>
                                            <div class="comment-time">
                                                <h6>50 mins ago</h6>
                                            </div>
                                        </div>
                                        <div class="sub-comment">
                                            <div class="media">
                                                <a href="#" class="user-img bg-size blur-up lazyload" style="background-image: url(&quot;../assets/images/user-sm/3.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                                                    <img src="../assets/images/user-sm/3.jpg" class="img-fluid blur-up lazyload bg-img" alt="user" style="display: none;">
                                                </a>
                                                <div class="media-body">
                                                    <a href="#">
                                                        <h5>sufiya elija</h5>
                                                    </a>
                                                    <p>Thank You So Much ❤❤</p>
                                                    <ul class="comment-option">
                                                        <li><a href="#">like</a></li>
                                                        <li><a href="#">reply</a></li>
                                                        <li><a href="#">translate</a></li>
                                                    </ul>
                                                </div>
                                                <div class="comment-time">
                                                    <h6>50 mins ago</h6>
                                                </div>
                                            </div>
                                            <div class="media">
                                                <a href="#" class="user-img bg-size blur-up lazyload" style="background-image: url(&quot;../assets/images/user-sm/4.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                                                    <img src="../assets/images/user-sm/4.jpg" class="img-fluid blur-up lazyload bg-img" alt="user" style="display: none;">
                                                </a>
                                                <div class="media-body">
                                                    <a href="#">
                                                        <h5>sufiya elija</h5>
                                                    </a>
                                                    <p>Thank You So Much ❤❤</p>
                                                    <ul class="comment-option">
                                                        <li><a href="#">like</a></li>
                                                        <li><a href="#">reply</a></li>
                                                        <li><a href="#">translate</a></li>
                                                    </ul>
                                                </div>
                                                <div class="comment-time">
                                                    <h6>50 mins ago</h6>
                                                </div>
                                            </div>
                                            <a href="javascript:void(0)" class="loader">
                                                <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-rotate-cw iw-15 ih-15"><polyline points="23 4 23 10 17 10"></polyline><path d="M20.49 15a9 9 0 1 1-2.12-9.36L23 10"></path></svg> load more
                                                replies
                                            </a>
                                        </div>
                                    </div>
                                    <div class="main-comment">
                                        <div class="media">
                                            <a href="#" class="user-img bg-size blur-up lazyload" style="background-image: url(&quot;../assets/images/user-sm/2.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                                                <img src="../assets/images/user-sm/2.jpg" class="img-fluid blur-up lazyload bg-img" alt="user" style="display: none;">
                                            </a>
                                            <div class="media-body">
                                                <a href="#">
                                                    <h5>Pabelo Mukrani</h5>
                                                </a>
                                                <p>It’s party time, Sufiya..... and happy birthday cuty 🎉🎊</p>
                                                <ul class="comment-option">
                                                    <li><a href="#">like</a></li>
                                                    <li><a href="#">reply</a></li>
                                                    <li><a href="#">translate</a></li>
                                                </ul>
                                            </div>
                                            <div class="comment-time">
                                                <h6>50 mins ago</h6>
                                            </div>
                                        </div>
                                    </div>
                                </div>
                                <div class="reply">
                                    <div class="search-input input-style input-lg icon-right">
                                        <input type="text" class="form-control emojiPicker" placeholder="write a comment..">
                                        <a href="javascript:void(0)">
                                            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-smile icon icon-2 iw-14 ih-14"><circle cx="12" cy="12" r="10"></circle><path d="M8 14s1.5 2 4 2 4-2 4-2"></path><line x1="9" y1="9" x2="9.01" y2="9"></line><line x1="15" y1="9" x2="15.01" y2="9"></line></svg>
                                        </a>
                                        <a href="javascript:void(0)">
                                            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-camera icon iw-14 ih-14"><path d="M23 19a2 2 0 0 1-2 2H3a2 2 0 0 1-2-2V8a2 2 0 0 1 2-2h4l2-3h6l2 3h4a2 2 0 0 1 2 2z"></path><circle cx="12" cy="13" r="4"></circle></svg>
                                        </a>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                    <div class="post-wrapper col-grid-box section-t-space" style="display: block;">
                        <div class="post-title">
                            <div class="profile">
                                <div class="media">
                                    <a class="popover-cls user-img bg-size blur-up lazyload" data-bs-toggle="popover" data-placement="right" data-name="sufiya eliza" data-img="../assets/images/user-sm/11.jpg" style="background-image: url(&quot;../assets/images/user-sm/11.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;" data-bs-original-title="" title="">
                                        <img src="../assets/images/user-sm/11.jpg" class="img-fluid blur-up lazyload bg-img" alt="user" style="display: none;">
                                    </a>
                                    <div class="media-body">
                                        <h5>sufiya eliza</h5>
                                        <h6>30 mins ago</h6>
                                    </div>
                                </div>
                            </div>
                            <div class="setting-btn ms-auto setting-dropdown no-bg">
                                <div class="btn-group custom-dropdown arrow-none dropdown-sm">
                                    <div role="button" data-bs-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
                                        <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-more-horizontal icon icon-font-color iw-14"><circle cx="12" cy="12" r="1"></circle><circle cx="19" cy="12" r="1"></circle><circle cx="5" cy="12" r="1"></circle></svg>
                                    </div>
                                    <div class="dropdown-menu dropdown-menu-right custom-dropdown">
                                        <ul>
                                            <li>
                                                <a href=""><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-bookmark icon-font-light iw-16 ih-16"><path d="M19 21l-7-5-7 5V5a2 2 0 0 1 2-2h10a2 2 0 0 1 2 2z"></path></svg>save post</a>
                                            </li>
                                            <li>
                                                <a href=""><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-edit icon-font-light iw-16 ih-16"><path d="M11 4H4a2 2 0 0 0-2 2v14a2 2 0 0 0 2 2h14a2 2 0 0 0 2-2v-7"></path><path d="M18.5 2.5a2.121 2.121 0 0 1 3 3L12 15l-4 1 1-4 9.5-9.5z"></path></svg>edit post</a>
                                            </li>
                                            <li>
                                                <a href=""><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-x-square icon-font-light iw-16 ih-16"><rect x="3" y="3" width="18" height="18" rx="2" ry="2"></rect><line x1="9" y1="9" x2="15" y2="15"></line><line x1="15" y1="9" x2="9" y2="15"></line></svg>hide post</a>
                                            </li>
                                        </ul>
                                    </div>
                                </div>
                            </div>
                        </div>
                        <div class="post-details">
                            <div class="img-wrapper">
                                <div style="width:100%;height:0;padding-bottom:56%;position:relative;"><iframe src="https://giphy.com/embed/xl2zRzM8sVo3td58kS" style="position:absolute" class="giphy-embed w-100 h-100" allowfullscreen=""></iframe></div>
                            </div>
                            <div class="detail-box">
                                <h3>Celebration new album song launched</h3>
                                <h5 class="tag"><span>#Musiccelebration,</span> #music, #party, #music</h5>
                                <p>Lorem Ipsum is simply dummy text of the printing and typesetting industry.
                                    has been the industry's standard dummy text ever since the 1500s</p>
                                <div class="bookmark favourite-btn">
                                    <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-bookmark iw-14 ih-14"><path d="M19 21l-7-5-7 5V5a2 2 0 0 1 2-2h10a2 2 0 0 1 2 2z"></path></svg>
                                </div>
                                <div class="people-likes">
                                    <ul>
                                        <li class="bg-size blur-up lazyload" style="background-image: url(&quot;../assets/images/user-sm/1.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                                            <img src="../assets/images/user-sm/1.jpg" class="img-fluid blur-up lazyload bg-img" alt="" style="display: none;">
                                        </li>
                                        <li class="bg-size blur-up lazyload" style="background-image: url(&quot;../assets/images/user-sm/2.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                                            <img src="../assets/images/user-sm/2.jpg" class="img-fluid blur-up lazyload bg-img" alt="" style="display: none;">
                                        </li>
                                        <li class="bg-size blur-up lazyload" style="background-image: url(&quot;../assets/images/user-sm/3.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                                            <img src="../assets/images/user-sm/3.jpg" class="img-fluid blur-up lazyload bg-img" alt="" style="display: none;">
                                        </li>
                                    </ul>
                                    <h6>+12 people react this post</h6>
                                </div>
                            </div>
                            <div class="like-panel">
                                <div class="left-emoji">
                                    <ul>
                                        <li>
                                            <img src="../assets/svg/emoji/040.svg" alt="smile">
                                        </li>
                                        <li>
                                            <img src="../assets/svg/emoji/113.svg" alt="heart">
                                        </li>
                                        <li>
                                            <img src="../assets/svg/emoji/027.svg" alt="cry">
                                        </li>
                                        <li>
                                            <img src="../assets/svg/emoji/033.svg" alt="angry">
                                        </li>
                                    </ul>
                                    <h6>+75</h6>
                                </div>
                                <div class="right-stats">
                                    <ul>
                                        <li>
                                            <h5>
                                                <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-message-square iw-16 ih-16"><path d="M21 15a2 2 0 0 1-2 2H7l-4 4V5a2 2 0 0 1 2-2h14a2 2 0 0 1 2 2z"></path></svg>
                                                <span>4565</span> comment
                                            </h5>
                                        </li>
                                        <li>
                                            <h5>
                                                <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-share iw-16 ih-16"><path d="M4 12v8a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2v-8"></path><polyline points="16 6 12 2 8 6"></polyline><line x1="12" y1="2" x2="12" y2="15"></line></svg><span>985</span>
                                                share
                                            </h5>
                                        </li>
                                    </ul>
                                </div>
                            </div>
                            <div class="post-react">
                                <ul>
                                    <li class="react-btn">
                                        <a class="react-click" href="javascript:void(0)">
                                            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-smile iw-18 ih-18"><circle cx="12" cy="12" r="10"></circle><path d="M8 14s1.5 2 4 2 4-2 4-2"></path><line x1="9" y1="9" x2="9.01" y2="9"></line><line x1="15" y1="9" x2="15.01" y2="9"></line></svg> react
                                        </a>
                                        <div class="react-box">
                                            <ul>
                                                <li data-title="smile">
                                                    <a href="javascript:void(0)">
                                                        <img src="../assets/svg/emoji/040.svg" alt="smile">
                                                    </a>
                                                </li>
                                                <li data-title="love">
                                                    <a href="javascript:void(0)">
                                                        <img src="../assets/svg/emoji/113.svg" alt="heart">
                                                    </a>
                                                </li>
                                                <li data-title="cry">
                                                    <a href="javascript:void(0)">
                                                        <img src="../assets/svg/emoji/027.svg" alt="cry">
                                                    </a>
                                                </li>
                                                <li data-title="wow">
                                                    <a href="javascript:void(0)">
                                                        <img src="../assets/svg/emoji/052.svg" alt="angry">
                                                    </a>
                                                </li>
                                                <li data-title="angry">
                                                    <a href="javascript:void(0)">
                                                        <img src="../assets/svg/emoji/039.svg" alt="angry">
                                                    </a>
                                                </li>
                                                <li data-title="haha">
                                                    <a href="javascript:void(0)">
                                                        <img src="../assets/svg/emoji/042.svg" alt="">
                                                    </a>
                                                </li>
                                            </ul>
                                        </div>
                                    </li>
                                    <li class="comment-click">
                                        <a href="javascript:void(0)">
                                            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-message-square iw-18 ih-18"><path d="M21 15a2 2 0 0 1-2 2H7l-4 4V5a2 2 0 0 1 2-2h14a2 2 0 0 1 2 2z"></path></svg> comment
                                        </a>
                                    </li>
                                    <li data-bs-target="#shareModal" data-bs-toggle="modal">
                                        <a href="javascript:void(0)">
                                            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-share iw-16 ih-16"><path d="M4 12v8a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2v-8"></path><polyline points="16 6 12 2 8 6"></polyline><line x1="12" y1="2" x2="12" y2="15"></line></svg> share
                                        </a>
                                    </li>
                                </ul>
                            </div>
                            <div class="comment-section">
                                <div class="comments d-none">
                                    <div class="ldr-comments">
                                        <ul>
                                            <li>
                                                <div class="media">
                                                    <div class="ldr-img"></div>
                                                    <div class="media-body">
                                                        <div class="contents">
                                                            <div class="ldr-content"></div>
                                                            <div class="ldr-content"></div>
                                                        </div>
                                                    </div>
                                                </div>
                                                <ul class="sub-comment">
                                                    <li>
                                                        <div class="media">
                                                            <div class="ldr-img"></div>
                                                            <div class="media-body">
                                                                <div class="contents">
                                                                    <div class="ldr-content"></div>
                                                                    <div class="ldr-content"></div>
                                                                </div>
                                                            </div>
                                                        </div>
                                                    </li>
                                                </ul>
                                            </li>
                                            <li>
                                                <div class="media">
                                                    <div class="ldr-img"></div>
                                                    <div class="media-body">
                                                        <div class="contents">
                                                            <div class="ldr-content"></div>
                                                            <div class="ldr-content"></div>
                                                        </div>
                                                    </div>
                                                </div>
                                            </li>
                                            <li>
                                                <div class="media">
                                                    <div class="ldr-img"></div>
                                                    <div class="media-body">
                                                        <div class="contents">
                                                            <div class="ldr-content"></div>
                                                            <div class="ldr-content"></div>
                                                        </div>
                                                    </div>
                                                </div>
                                            </li>
                                        </ul>
                                    </div>
                                    <div class="main-comment">
                                        <div class="media">
                                            <a href="#" class="user-img bg-size blur-up lazyload" style="background-image: url(&quot;../assets/images/user-sm/2.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                                                <img src="../assets/images/user-sm/2.jpg" class="img-fluid blur-up lazyload bg-img" alt="user" style="display: none;">
                                            </a>
                                            <div class="media-body">
                                                <a href="#">
                                                    <h5>Pabelo Mukrani</h5>
                                                </a>
                                                <p>Oooo Very Cute and Sweet Dog, happy birthday Cuty....
                                                    🙂
                                                </p>
                                                <ul class="comment-option">
                                                    <li><a href="#">like (5)</a></li>
                                                    <li><a href="#">reply</a></li>
                                                    <li><a href="#">translate</a></li>
                                                </ul>
                                            </div>
                                            <div class="comment-time">
                                                <h6>50 mins ago</h6>
                                            </div>
                                        </div>
                                        <div class="sub-comment">
                                            <div class="media">
                                                <a href="#" class="user-img bg-size blur-up lazyload" style="background-image: url(&quot;../assets/images/user-sm/3.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                                                    <img src="../assets/images/user-sm/3.jpg" class="img-fluid blur-up lazyload bg-img" alt="user" style="display: none;">
                                                </a>
                                                <div class="media-body">
                                                    <a href="#">
                                                        <h5>sufiya elija</h5>
                                                    </a>
                                                    <p>Thank You So Much ❤❤</p>
                                                    <ul class="comment-option">
                                                        <li><a href="#">like</a></li>
                                                        <li><a href="#">reply</a></li>
                                                        <li><a href="#">translate</a></li>
                                                    </ul>
                                                </div>
                                                <div class="comment-time">
                                                    <h6>50 mins ago</h6>
                                                </div>
                                            </div>
                                            <div class="media">
                                                <a href="#" class="user-img bg-size blur-up lazyload" style="background-image: url(&quot;../assets/images/user-sm/4.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                                                    <img src="../assets/images/user-sm/4.jpg" class="img-fluid blur-up lazyload bg-img" alt="user" style="display: none;">
                                                </a>
                                                <div class="media-body">
                                                    <a href="#">
                                                        <h5>sufiya elija</h5>
                                                    </a>
                                                    <p>Thank You So Much ❤❤</p>
                                                    <ul class="comment-option">
                                                        <li><a href="#">like</a></li>
                                                        <li><a href="#">reply</a></li>
                                                        <li><a href="#">translate</a></li>
                                                    </ul>
                                                </div>
                                                <div class="comment-time">
                                                    <h6>50 mins ago</h6>
                                                </div>
                                            </div>
                                            <a href="javascript:void(0)" class="loader">
                                                <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-rotate-cw iw-15 ih-15"><polyline points="23 4 23 10 17 10"></polyline><path d="M20.49 15a9 9 0 1 1-2.12-9.36L23 10"></path></svg> load more
                                                replies
                                            </a>
                                        </div>
                                    </div>
                                    <div class="main-comment">
                                        <div class="media">
                                            <a href="#" class="user-img bg-size blur-up lazyload" style="background-image: url(&quot;../assets/images/user-sm/2.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                                                <img src="../assets/images/user-sm/2.jpg" class="img-fluid blur-up lazyload bg-img" alt="user" style="display: none;">
                                            </a>
                                            <div class="media-body">
                                                <a href="#">
                                                    <h5>Pabelo Mukrani</h5>
                                                </a>
                                                <p>It’s party time, Sufiya..... and happy birthday cuty 🎉🎊</p>
                                                <ul class="comment-option">
                                                    <li><a href="#">like</a></li>
                                                    <li><a href="#">reply</a></li>
                                                    <li><a href="#">translate</a></li>
                                                </ul>
                                            </div>
                                            <div class="comment-time">
                                                <h6>50 mins ago</h6>
                                            </div>
                                        </div>
                                    </div>
                                </div>
                                <div class="reply">
                                    <div class="search-input input-style input-lg icon-right">
                                        <input type="text" class="form-control emojiPicker" placeholder="write a comment..">
                                        <a href="javascript:void(0)">
                                            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-smile icon icon-2 iw-14 ih-14"><circle cx="12" cy="12" r="10"></circle><path d="M8 14s1.5 2 4 2 4-2 4-2"></path><line x1="9" y1="9" x2="9.01" y2="9"></line><line x1="15" y1="9" x2="15.01" y2="9"></line></svg>
                                        </a>
                                        <a href="javascript:void(0)">
                                            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-camera icon iw-14 ih-14"><path d="M23 19a2 2 0 0 1-2 2H3a2 2 0 0 1-2-2V8a2 2 0 0 1 2-2h4l2-3h6l2 3h4a2 2 0 0 1 2 2z"></path><circle cx="12" cy="13" r="4"></circle></svg>
                                        </a>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                    <div class="post-wrapper col-grid-box section-t-space" style="display: block;">
                        <div class="post-title">
                            <div class="profile">
                                <div class="media">
                                    <a class="popover-cls user-img bg-size blur-up lazyload" data-bs-toggle="popover" data-placement="right" data-name="sufiya eliza" data-img="../assets/images/user-sm/15.jpg" style="background-image: url(&quot;../assets/images/user-sm/15.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;" data-bs-original-title="" title="">
                                        <img src="../assets/images/user-sm/15.jpg" class="img-fluid blur-up lazyload bg-img" alt="user" style="display: none;">
                                    </a>
                                    <div class="media-body">
                                        <h5>sufiya eliza</h5>
                                        <h6>30 mins ago</h6>
                                    </div>
                                </div>
                            </div>
                            <div class="setting-btn ms-auto setting-dropdown no-bg">
                                <div class="btn-group custom-dropdown arrow-none dropdown-sm">
                                    <div role="button" data-bs-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
                                        <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-more-horizontal icon icon-font-color iw-14"><circle cx="12" cy="12" r="1"></circle><circle cx="19" cy="12" r="1"></circle><circle cx="5" cy="12" r="1"></circle></svg>
                                    </div>
                                    <div class="dropdown-menu dropdown-menu-right custom-dropdown">
                                        <ul>
                                            <li>
                                                <a href=""><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-bookmark icon-font-light iw-16 ih-16"><path d="M19 21l-7-5-7 5V5a2 2 0 0 1 2-2h10a2 2 0 0 1 2 2z"></path></svg>save post</a>
                                            </li>
                                            <li>
                                                <a href=""><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-edit icon-font-light iw-16 ih-16"><path d="M11 4H4a2 2 0 0 0-2 2v14a2 2 0 0 0 2 2h14a2 2 0 0 0 2-2v-7"></path><path d="M18.5 2.5a2.121 2.121 0 0 1 3 3L12 15l-4 1 1-4 9.5-9.5z"></path></svg>edit post</a>
                                            </li>
                                            <li>
                                                <a href=""><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-x-square icon-font-light iw-16 ih-16"><rect x="3" y="3" width="18" height="18" rx="2" ry="2"></rect><line x1="9" y1="9" x2="15" y2="15"></line><line x1="15" y1="9" x2="9" y2="15"></line></svg>hide post</a>
                                            </li>
                                        </ul>
                                    </div>
                                </div>
                            </div>
                        </div>
                        <div class="post-details ratio_55">
                            <div class="detail-box">
                                <h3>Celebration new album song launched</h3>
                                <h5 class="tag"><span>#Musiccelebration,</span> #music, #party, #music</h5>
                                <p>Lorem Ipsum is simply dummy text of the printing and typesetting industry.
                                    has been the industry's standard dummy text ever since the 1500s</p>
                                <div class="bookmark favourite-btn">
                                    <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-bookmark iw-14 ih-14"><path d="M19 21l-7-5-7 5V5a2 2 0 0 1 2-2h10a2 2 0 0 1 2 2z"></path></svg>
                                </div>
                                <div class="people-likes">
                                    <ul>
                                        <li class="bg-size blur-up lazyload" style="background-image: url(&quot;../assets/images/user-sm/1.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                                            <img src="../assets/images/user-sm/1.jpg" class="img-fluid blur-up lazyload bg-img" alt="" style="display: none;">
                                        </li>
                                        <li class="bg-size blur-up lazyload" style="background-image: url(&quot;../assets/images/user-sm/2.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                                            <img src="../assets/images/user-sm/2.jpg" class="img-fluid blur-up lazyload bg-img" alt="" style="display: none;">
                                        </li>
                                        <li class="bg-size blur-up lazyload" style="background-image: url(&quot;../assets/images/user-sm/3.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                                            <img src="../assets/images/user-sm/3.jpg" class="img-fluid blur-up lazyload bg-img" alt="" style="display: none;">
                                        </li>
                                    </ul>
                                    <h6>+12 people react this post</h6>
                                </div>
                            </div>
                            <div class="like-panel">
                                <div class="left-emoji">
                                    <ul>
                                        <li>
                                            <img src="../assets/svg/emoji/040.svg" alt="smile">
                                        </li>
                                        <li>
                                            <img src="../assets/svg/emoji/113.svg" alt="heart">
                                        </li>
                                        <li>
                                            <img src="../assets/svg/emoji/027.svg" alt="cry">
                                        </li>
                                        <li>
                                            <img src="../assets/svg/emoji/033.svg" alt="angry">
                                        </li>
                                    </ul>
                                    <h6>+75</h6>
                                </div>
                                <div class="right-stats">
                                    <ul>
                                        <li>
                                            <h5>
                                                <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-message-square iw-16 ih-16"><path d="M21 15a2 2 0 0 1-2 2H7l-4 4V5a2 2 0 0 1 2-2h14a2 2 0 0 1 2 2z"></path></svg>
                                                <span>4565</span> comment
                                            </h5>
                                        </li>
                                        <li>
                                            <h5>
                                                <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-share iw-16 ih-16"><path d="M4 12v8a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2v-8"></path><polyline points="16 6 12 2 8 6"></polyline><line x1="12" y1="2" x2="12" y2="15"></line></svg><span>985</span>
                                                share
                                            </h5>
                                        </li>
                                    </ul>
                                </div>
                            </div>
                            <div class="post-react">
                                <ul>
                                    <li class="react-btn">
                                        <a class="react-click" href="javascript:void(0)">
                                            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-smile iw-18 ih-18"><circle cx="12" cy="12" r="10"></circle><path d="M8 14s1.5 2 4 2 4-2 4-2"></path><line x1="9" y1="9" x2="9.01" y2="9"></line><line x1="15" y1="9" x2="15.01" y2="9"></line></svg> react
                                        </a>
                                        <div class="react-box">
                                            <ul>
                                                <li data-title="smile">
                                                    <a href="javascript:void(0)">
                                                        <img src="../assets/svg/emoji/040.svg" alt="smile">
                                                    </a>
                                                </li>
                                                <li data-title="love">
                                                    <a href="javascript:void(0)">
                                                        <img src="../assets/svg/emoji/113.svg" alt="heart">
                                                    </a>
                                                </li>
                                                <li data-title="cry">
                                                    <a href="javascript:void(0)">
                                                        <img src="../assets/svg/emoji/027.svg" alt="cry">
                                                    </a>
                                                </li>
                                                <li data-title="wow">
                                                    <a href="javascript:void(0)">
                                                        <img src="../assets/svg/emoji/052.svg" alt="angry">
                                                    </a>
                                                </li>
                                                <li data-title="angry">
                                                    <a href="javascript:void(0)">
                                                        <img src="../assets/svg/emoji/039.svg" alt="angry">
                                                    </a>
                                                </li>
                                                <li data-title="haha">
                                                    <a href="javascript:void(0)">
                                                        <img src="../assets/svg/emoji/042.svg" alt="">
                                                    </a>
                                                </li>
                                            </ul>
                                        </div>
                                    </li>
                                    <li class="comment-click">
                                        <a href="javascript:void(0)">
                                            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-message-square iw-18 ih-18"><path d="M21 15a2 2 0 0 1-2 2H7l-4 4V5a2 2 0 0 1 2-2h14a2 2 0 0 1 2 2z"></path></svg> comment
                                        </a>
                                    </li>
                                    <li data-bs-target="#shareModal" data-bs-toggle="modal">
                                        <a href="javascript:void(0)">
                                            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-share iw-16 ih-16"><path d="M4 12v8a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2v-8"></path><polyline points="16 6 12 2 8 6"></polyline><line x1="12" y1="2" x2="12" y2="15"></line></svg> share
                                        </a>
                                    </li>
                                </ul>
                            </div>
                            <div class="comment-section">
                                <div class="comments d-none">
                                    <div class="ldr-comments">
                                        <ul>
                                            <li>
                                                <div class="media">
                                                    <div class="ldr-img"></div>
                                                    <div class="media-body">
                                                        <div class="contents">
                                                            <div class="ldr-content"></div>
                                                            <div class="ldr-content"></div>
                                                        </div>
                                                    </div>
                                                </div>
                                                <ul class="sub-comment">
                                                    <li>
                                                        <div class="media">
                                                            <div class="ldr-img"></div>
                                                            <div class="media-body">
                                                                <div class="contents">
                                                                    <div class="ldr-content"></div>
                                                                    <div class="ldr-content"></div>
                                                                </div>
                                                            </div>
                                                        </div>
                                                    </li>
                                                </ul>
                                            </li>
                                            <li>
                                                <div class="media">
                                                    <div class="ldr-img"></div>
                                                    <div class="media-body">
                                                        <div class="contents">
                                                            <div class="ldr-content"></div>
                                                            <div class="ldr-content"></div>
                                                        </div>
                                                    </div>
                                                </div>
                                            </li>
                                            <li>
                                                <div class="media">
                                                    <div class="ldr-img"></div>
                                                    <div class="media-body">
                                                        <div class="contents">
                                                            <div class="ldr-content"></div>
                                                            <div class="ldr-content"></div>
                                                        </div>
                                                    </div>
                                                </div>
                                            </li>
                                        </ul>
                                    </div>
                                    <div class="main-comment">
                                        <div class="media">
                                            <a href="#" class="user-img bg-size blur-up lazyload" style="background-image: url(&quot;../assets/images/user-sm/2.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                                                <img src="../assets/images/user-sm/2.jpg" class="img-fluid blur-up lazyload bg-img" alt="user" style="display: none;">
                                            </a>
                                            <div class="media-body">
                                                <a href="#">
                                                    <h5>Pabelo Mukrani</h5>
                                                </a>
                                                <p>Oooo Very Cute and Sweet Dog, happy birthday Cuty....
                                                    🙂
                                                </p>
                                                <ul class="comment-option">
                                                    <li><a href="#">like (5)</a></li>
                                                    <li><a href="#">reply</a></li>
                                                    <li><a href="#">translate</a></li>
                                                </ul>
                                            </div>
                                            <div class="comment-time">
                                                <h6>50 mins ago</h6>
                                            </div>
                                        </div>
                                        <div class="sub-comment">
                                            <div class="media">
                                                <a href="#" class="user-img bg-size blur-up lazyload" style="background-image: url(&quot;../assets/images/user-sm/3.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                                                    <img src="../assets/images/user-sm/3.jpg" class="img-fluid blur-up lazyload bg-img" alt="user" style="display: none;">
                                                </a>
                                                <div class="media-body">
                                                    <a href="#">
                                                        <h5>sufiya elija</h5>
                                                    </a>
                                                    <p>Thank You So Much ❤❤</p>
                                                    <ul class="comment-option">
                                                        <li><a href="#">like</a></li>
                                                        <li><a href="#">reply</a></li>
                                                        <li><a href="#">translate</a></li>
                                                    </ul>
                                                </div>
                                                <div class="comment-time">
                                                    <h6>50 mins ago</h6>
                                                </div>
                                            </div>
                                            <div class="media">
                                                <a href="#" class="user-img bg-size blur-up lazyload" style="background-image: url(&quot;../assets/images/user-sm/4.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                                                    <img src="../assets/images/user-sm/4.jpg" class="img-fluid blur-up lazyload bg-img" alt="user" style="display: none;">
                                                </a>
                                                <div class="media-body">
                                                    <a href="#">
                                                        <h5>sufiya elija</h5>
                                                    </a>
                                                    <p>Thank You So Much ❤❤</p>
                                                    <ul class="comment-option">
                                                        <li><a href="#">like</a></li>
                                                        <li><a href="#">reply</a></li>
                                                        <li><a href="#">translate</a></li>
                                                    </ul>
                                                </div>
                                                <div class="comment-time">
                                                    <h6>50 mins ago</h6>
                                                </div>
                                            </div>
                                            <a href="javascript:void(0)" class="loader">
                                                <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-rotate-cw iw-15 ih-15"><polyline points="23 4 23 10 17 10"></polyline><path d="M20.49 15a9 9 0 1 1-2.12-9.36L23 10"></path></svg> load more
                                                replies
                                            </a>
                                        </div>
                                    </div>
                                    <div class="main-comment">
                                        <div class="media">
                                            <a href="#" class="user-img bg-size blur-up lazyload" style="background-image: url(&quot;../assets/images/user-sm/2.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                                                <img src="../assets/images/user-sm/2.jpg" class="img-fluid blur-up lazyload bg-img" alt="user" style="display: none;">
                                            </a>
                                            <div class="media-body">
                                                <a href="#">
                                                    <h5>Pabelo Mukrani</h5>
                                                </a>
                                                <p>It’s party time, Sufiya..... and happy birthday cuty 🎉🎊</p>
                                                <ul class="comment-option">
                                                    <li><a href="#">like</a></li>
                                                    <li><a href="#">reply</a></li>
                                                    <li><a href="#">translate</a></li>
                                                </ul>
                                            </div>
                                            <div class="comment-time">
                                                <h6>50 mins ago</h6>
                                            </div>
                                        </div>
                                    </div>
                                </div>
                                <div class="reply">
                                    <div class="search-input input-style input-lg icon-right">
                                        <input type="text" class="form-control emojiPicker" placeholder="write a comment..">
                                        <a href="javascript:void(0)">
                                            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-smile icon icon-2 iw-14 ih-14"><circle cx="12" cy="12" r="10"></circle><path d="M8 14s1.5 2 4 2 4-2 4-2"></path><line x1="9" y1="9" x2="9.01" y2="9"></line><line x1="15" y1="9" x2="15.01" y2="9"></line></svg>
                                        </a>
                                        <a href="javascript:void(0)">
                                            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-camera icon iw-14 ih-14"><path d="M23 19a2 2 0 0 1-2 2H3a2 2 0 0 1-2-2V8a2 2 0 0 1 2-2h4l2-3h6l2 3h4a2 2 0 0 1 2 2z"></path><circle cx="12" cy="13" r="4"></circle></svg>
                                        </a>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                    <div class="post-wrapper col-grid-box section-t-space">
                        <div class="post-title">
                            <div class="profile">
                                <div class="media">
                                    <a class="popover-cls user-img bg-size blur-up lazyload" data-bs-toggle="popover" data-placement="right" data-name="sufiya eliza" data-img="../assets/images/user-sm/15.jpg" style="background-image: url(&quot;../assets/images/user-sm/15.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;" data-bs-original-title="" title="">
                                        <img src="../assets/images/user-sm/15.jpg" class="img-fluid blur-up lazyload bg-img" alt="user" style="display: none;">
                                    </a>
                                    <div class="media-body">
                                        <h5>sufiya eliza</h5>
                                        <h6>30 mins ago</h6>
                                    </div>
                                </div>
                            </div>
                            <div class="setting-btn ms-auto setting-dropdown no-bg">
                                <div class="btn-group custom-dropdown arrow-none dropdown-sm">
                                    <div role="button" data-bs-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
                                        <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-more-horizontal icon icon-font-color iw-14"><circle cx="12" cy="12" r="1"></circle><circle cx="19" cy="12" r="1"></circle><circle cx="5" cy="12" r="1"></circle></svg>
                                    </div>
                                    <div class="dropdown-menu dropdown-menu-right custom-dropdown">
                                        <ul>
                                            <li>
                                                <a href=""><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-bookmark icon-font-light iw-16 ih-16"><path d="M19 21l-7-5-7 5V5a2 2 0 0 1 2-2h10a2 2 0 0 1 2 2z"></path></svg>save post</a>
                                            </li>
                                            <li>
                                                <a href=""><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-edit icon-font-light iw-16 ih-16"><path d="M11 4H4a2 2 0 0 0-2 2v14a2 2 0 0 0 2 2h14a2 2 0 0 0 2-2v-7"></path><path d="M18.5 2.5a2.121 2.121 0 0 1 3 3L12 15l-4 1 1-4 9.5-9.5z"></path></svg>edit post</a>
                                            </li>
                                            <li>
                                                <a href=""><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-x-square icon-font-light iw-16 ih-16"><rect x="3" y="3" width="18" height="18" rx="2" ry="2"></rect><line x1="9" y1="9" x2="15" y2="15"></line><line x1="15" y1="9" x2="9" y2="15"></line></svg>hide post</a>
                                            </li>
                                        </ul>
                                    </div>
                                </div>
                            </div>
                        </div>
                        <div class="post-details">
                            <a class="popover-cls user-img bg-size blur-up lazyload" data-bs-toggle="popover" data-placement="right" data-name="sufiya eliza" data-img="../assets/images/user-sm/2.jpg" style="background-image: url(&quot;../assets/images/user-sm/2.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;" data-bs-original-title="" title="">
                                <img src="../assets/images/user-sm/2.jpg" class="img-fluid blur-up lazyload bg-img" alt="user" style="display: none;">
                            </a>
                            <div class="detail-box">
                                <h3>Celebration new album song launched</h3>
                                <h5 class="tag"><span>#Musiccelebration,</span> #music, #party, #music</h5>
                                <p>Lorem Ipsum is simply dummy text of the printing and typesetting industry.
                                    has been the industry's standard dummy text ever since the 1500s</p>
                                <div class="bookmark favourite-btn">
                                    <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-bookmark iw-14 ih-14"><path d="M19 21l-7-5-7 5V5a2 2 0 0 1 2-2h10a2 2 0 0 1 2 2z"></path></svg>
                                </div>
                                <div class="people-likes">
                                    <ul>
                                        <li class="bg-size blur-up lazyload" style="background-image: url(&quot;../assets/images/user-sm/1.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                                            <img src="../assets/images/user-sm/1.jpg" class="img-fluid blur-up lazyload bg-img" alt="" style="display: none;">
                                        </li>
                                        <li class="bg-size blur-up lazyload" style="background-image: url(&quot;../assets/images/user-sm/2.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                                            <img src="../assets/images/user-sm/2.jpg" class="img-fluid blur-up lazyload bg-img" alt="" style="display: none;">
                                        </li>
                                        <li class="bg-size blur-up lazyload" style="background-image: url(&quot;../assets/images/user-sm/3.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                                            <img src="../assets/images/user-sm/3.jpg" class="img-fluid blur-up lazyload bg-img" alt="" style="display: none;">
                                        </li>
                                    </ul>
                                    <h6>+12 people react this post</h6>
                                </div>
                            </div>
                            <div class="like-panel">
                                <div class="left-emoji">
                                    <ul>
                                        <li>
                                            <img src="../assets/svg/emoji/040.svg" alt="smile">
                                        </li>
                                        <li>
                                            <img src="../assets/svg/emoji/113.svg" alt="heart">
                                        </li>
                                        <li>
                                            <img src="../assets/svg/emoji/027.svg" alt="cry">
                                        </li>
                                        <li>
                                            <img src="../assets/svg/emoji/033.svg" alt="angry">
                                        </li>
                                    </ul>
                                    <h6>+75</h6>
                                </div>
                                <div class="right-stats">
                                    <ul>
                                        <li>
                                            <h5>
                                                <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-message-square iw-16 ih-16"><path d="M21 15a2 2 0 0 1-2 2H7l-4 4V5a2 2 0 0 1 2-2h14a2 2 0 0 1 2 2z"></path></svg>
                                                <span>4565</span> comment
                                            </h5>
                                        </li>
                                        <li>
                                            <h5>
                                                <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-share iw-16 ih-16"><path d="M4 12v8a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2v-8"></path><polyline points="16 6 12 2 8 6"></polyline><line x1="12" y1="2" x2="12" y2="15"></line></svg><span>985</span>
                                                share
                                            </h5>
                                        </li>
                                    </ul>
                                </div>
                            </div>
                            <div class="post-react">
                                <ul>
                                    <li class="react-btn">
                                        <a class="react-click" href="javascript:void(0)">
                                            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-smile iw-18 ih-18"><circle cx="12" cy="12" r="10"></circle><path d="M8 14s1.5 2 4 2 4-2 4-2"></path><line x1="9" y1="9" x2="9.01" y2="9"></line><line x1="15" y1="9" x2="15.01" y2="9"></line></svg> react
                                        </a>
                                        <div class="react-box">
                                            <ul>
                                                <li data-title="smile">
                                                    <a href="javascript:void(0)">
                                                        <img src="../assets/svg/emoji/040.svg" alt="smile">
                                                    </a>
                                                </li>
                                                <li data-title="love">
                                                    <a href="javascript:void(0)">
                                                        <img src="../assets/svg/emoji/113.svg" alt="heart">
                                                    </a>
                                                </li>
                                                <li data-title="cry">
                                                    <a href="javascript:void(0)">
                                                        <img src="../assets/svg/emoji/027.svg" alt="cry">
                                                    </a>
                                                </li>
                                                <li data-title="wow">
                                                    <a href="javascript:void(0)">
                                                        <img src="../assets/svg/emoji/052.svg" alt="angry">
                                                    </a>
                                                </li>
                                                <li data-title="angry">
                                                    <a href="javascript:void(0)">
                                                        <img src="../assets/svg/emoji/039.svg" alt="angry">
                                                    </a>
                                                </li>
                                                <li data-title="haha">
                                                    <a href="javascript:void(0)">
                                                        <img src="../assets/svg/emoji/042.svg" alt="">
                                                    </a>
                                                </li>
                                            </ul>
                                        </div>
                                    </li>
                                    <li class="comment-click">
                                        <a href="javascript:void(0)">
                                            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-message-square iw-18 ih-18"><path d="M21 15a2 2 0 0 1-2 2H7l-4 4V5a2 2 0 0 1 2-2h14a2 2 0 0 1 2 2z"></path></svg> comment
                                        </a>
                                    </li>
                                    <li data-bs-target="#shareModal" data-bs-toggle="modal">
                                        <a href="javascript:void(0)">
                                            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-share iw-16 ih-16"><path d="M4 12v8a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2v-8"></path><polyline points="16 6 12 2 8 6"></polyline><line x1="12" y1="2" x2="12" y2="15"></line></svg> share
                                        </a>
                                    </li>
                                </ul>
                            </div>
                            <div class="comment-section">
                                <div class="comments d-none">
                                    <div class="ldr-comments">
                                        <ul>
                                            <li>
                                                <div class="media">
                                                    <div class="ldr-img"></div>
                                                    <div class="media-body">
                                                        <div class="contents">
                                                            <div class="ldr-content"></div>
                                                            <div class="ldr-content"></div>
                                                        </div>
                                                    </div>
                                                </div>
                                                <ul class="sub-comment">
                                                    <li>
                                                        <div class="media">
                                                            <div class="ldr-img"></div>
                                                            <div class="media-body">
                                                                <div class="contents">
                                                                    <div class="ldr-content"></div>
                                                                    <div class="ldr-content"></div>
                                                                </div>
                                                            </div>
                                                        </div>
                                                    </li>
                                                </ul>
                                            </li>
                                            <li>
                                                <div class="media">
                                                    <div class="ldr-img"></div>
                                                    <div class="media-body">
                                                        <div class="contents">
                                                            <div class="ldr-content"></div>
                                                            <div class="ldr-content"></div>
                                                        </div>
                                                    </div>
                                                </div>
                                            </li>
                                            <li>
                                                <div class="media">
                                                    <div class="ldr-img"></div>
                                                    <div class="media-body">
                                                        <div class="contents">
                                                            <div class="ldr-content"></div>
                                                            <div class="ldr-content"></div>
                                                        </div>
                                                    </div>
                                                </div>
                                            </li>
                                        </ul>
                                    </div>
                                    <div class="main-comment">
                                        <div class="media">
                                            <a href="#" class="user-img bg-size blur-up lazyload" style="background-image: url(&quot;../assets/images/user-sm/2.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                                                <img src="../assets/images/user-sm/2.jpg" class="img-fluid blur-up lazyload bg-img" alt="user" style="display: none;">
                                            </a>
                                            <div class="media-body">
                                                <a href="#">
                                                    <h5>Pabelo Mukrani</h5>
                                                </a>
                                                <p>Oooo Very Cute and Sweet Dog, happy birthday Cuty....
                                                    🙂
                                                </p>
                                                <ul class="comment-option">
                                                    <li><a href="#">like (5)</a></li>
                                                    <li><a href="#">reply</a></li>
                                                    <li><a href="#">translate</a></li>
                                                </ul>
                                            </div>
                                            <div class="comment-time">
                                                <h6>50 mins ago</h6>
                                            </div>
                                        </div>
                                        <div class="sub-comment">
                                            <div class="media">
                                                <a href="#" class="user-img bg-size blur-up lazyload" style="background-image: url(&quot;../assets/images/user-sm/3.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                                                    <img src="../assets/images/user-sm/3.jpg" class="img-fluid blur-up lazyload bg-img" alt="user" style="display: none;">
                                                </a>
                                                <div class="media-body">
                                                    <a href="#">
                                                        <h5>sufiya elija</h5>
                                                    </a>
                                                    <p>Thank You So Much ❤❤</p>
                                                    <ul class="comment-option">
                                                        <li><a href="#">like</a></li>
                                                        <li><a href="#">reply</a></li>
                                                        <li><a href="#">translate</a></li>
                                                    </ul>
                                                </div>
                                                <div class="comment-time">
                                                    <h6>50 mins ago</h6>
                                                </div>
                                            </div>
                                            <div class="media">
                                                <a href="#" class="user-img bg-size blur-up lazyload" style="background-image: url(&quot;../assets/images/user-sm/4.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                                                    <img src="../assets/images/user-sm/4.jpg" class="img-fluid blur-up lazyload bg-img" alt="user" style="display: none;">
                                                </a>
                                                <div class="media-body">
                                                    <a href="#">
                                                        <h5>sufiya elija</h5>
                                                    </a>
                                                    <p>Thank You So Much ❤❤</p>
                                                    <ul class="comment-option">
                                                        <li><a href="#">like</a></li>
                                                        <li><a href="#">reply</a></li>
                                                        <li><a href="#">translate</a></li>
                                                    </ul>
                                                </div>
                                                <div class="comment-time">
                                                    <h6>50 mins ago</h6>
                                                </div>
                                            </div>
                                            <a href="javascript:void(0)" class="loader">
                                                <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-rotate-cw iw-15 ih-15"><polyline points="23 4 23 10 17 10"></polyline><path d="M20.49 15a9 9 0 1 1-2.12-9.36L23 10"></path></svg> load more
                                                replies
                                            </a>
                                        </div>
                                    </div>
                                    <div class="main-comment">
                                        <div class="media">
                                            <a href="#" class="user-img bg-size blur-up lazyload" style="background-image: url(&quot;../assets/images/user-sm/2.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                                                <img src="../assets/images/user-sm/2.jpg" class="img-fluid blur-up lazyload bg-img" alt="user" style="display: none;">
                                            </a>
                                            <div class="media-body">
                                                <a href="#">
                                                    <h5>Pabelo Mukrani</h5>
                                                </a>
                                                <p>It’s party time, Sufiya..... and happy birthday cuty 🎉🎊</p>
                                                <ul class="comment-option">
                                                    <li><a href="#">like</a></li>
                                                    <li><a href="#">reply</a></li>
                                                    <li><a href="#">translate</a></li>
                                                </ul>
                                            </div>
                                            <div class="comment-time">
                                                <h6>50 mins ago</h6>
                                            </div>
                                        </div>
                                    </div>
                                </div>
                                <div class="reply">
                                    <div class="search-input input-style input-lg icon-right">
                                        <input type="text" class="form-control emojiPicker" placeholder="write a comment..">
                                        <a href="javascript:void(0)">
                                            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-smile icon icon-2 iw-14 ih-14"><circle cx="12" cy="12" r="10"></circle><path d="M8 14s1.5 2 4 2 4-2 4-2"></path><line x1="9" y1="9" x2="9.01" y2="9"></line><line x1="15" y1="9" x2="15.01" y2="9"></line></svg>
                                        </a>
                                        <a href="javascript:void(0)">
                                            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-camera icon iw-14 ih-14"><path d="M23 19a2 2 0 0 1-2 2H3a2 2 0 0 1-2-2V8a2 2 0 0 1 2-2h4l2-3h6l2 3h4a2 2 0 0 1 2 2z"></path><circle cx="12" cy="13" r="4"></circle></svg>
                                        </a>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                    <div class="post-wrapper col-grid-box section-t-space">
                        <div class="post-title">
                            <div class="profile">
                                <div class="media">
                                    <a class="popover-cls user-img bg-size blur-up lazyload" data-bs-toggle="popover" data-placement="right" data-name="sufiya eliza" data-img="../assets/images/user-sm/10.jpg" style="background-image: url(&quot;../assets/images/user-sm/10.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;" data-bs-original-title="" title="">
                                        <img src="../assets/images/user-sm/10.jpg" class="img-fluid blur-up lazyload bg-img" alt="user" style="display: none;">
                                    </a>
                                    <div class="media-body">
                                        <h5>sufiya eliza</h5>
                                        <h6>30 mins ago</h6>
                                    </div>
                                </div>
                            </div>
                            <div class="setting-btn ms-auto setting-dropdown no-bg">
                                <div class="btn-group custom-dropdown arrow-none dropdown-sm">
                                    <div role="button" data-bs-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
                                        <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-more-horizontal icon icon-font-color iw-14"><circle cx="12" cy="12" r="1"></circle><circle cx="19" cy="12" r="1"></circle><circle cx="5" cy="12" r="1"></circle></svg>
                                    </div>
                                    <div class="dropdown-menu dropdown-menu-right custom-dropdown">
                                        <ul>
                                            <li>
                                                <a href=""><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-bookmark icon-font-light iw-16 ih-16"><path d="M19 21l-7-5-7 5V5a2 2 0 0 1 2-2h10a2 2 0 0 1 2 2z"></path></svg>save post</a>
                                            </li>
                                            <li>
                                                <a href=""><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-edit icon-font-light iw-16 ih-16"><path d="M11 4H4a2 2 0 0 0-2 2v14a2 2 0 0 0 2 2h14a2 2 0 0 0 2-2v-7"></path><path d="M18.5 2.5a2.121 2.121 0 0 1 3 3L12 15l-4 1 1-4 9.5-9.5z"></path></svg>edit post</a>
                                            </li>
                                            <li>
                                                <a href=""><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-x-square icon-font-light iw-16 ih-16"><rect x="3" y="3" width="18" height="18" rx="2" ry="2"></rect><line x1="9" y1="9" x2="15" y2="15"></line><line x1="15" y1="9" x2="9" y2="15"></line></svg>hide post</a>
                                            </li>
                                        </ul>
                                    </div>
                                </div>
                            </div>
                        </div>
                        <div class="post-details ratio_55">
                            <div class="detail-box">
                                <h3>Celebration new album song launched</h3>
                                <h5 class="tag"><span>#Musiccelebration,</span> #music, #party, #music</h5>
                                <p>Lorem Ipsum is simply dummy text of the printing and typesetting industry.
                                    has been the industry's standard dummy text ever since the 1500s</p>
                                <div class="bookmark favourite-btn">
                                    <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-bookmark iw-14 ih-14"><path d="M19 21l-7-5-7 5V5a2 2 0 0 1 2-2h10a2 2 0 0 1 2 2z"></path></svg>
                                </div>
                                <div class="people-likes">
                                    <ul>
                                        <li class="bg-size blur-up lazyload" style="background-image: url(&quot;../assets/images/user-sm/1.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                                            <img src="../assets/images/user-sm/1.jpg" class="img-fluid blur-up lazyload bg-img" alt="" style="display: none;">
                                        </li>
                                        <li class="bg-size blur-up lazyload" style="background-image: url(&quot;../assets/images/user-sm/2.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                                            <img src="../assets/images/user-sm/2.jpg" class="img-fluid blur-up lazyload bg-img" alt="" style="display: none;">
                                        </li>
                                        <li class="bg-size blur-up lazyload" style="background-image: url(&quot;../assets/images/user-sm/3.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                                            <img src="../assets/images/user-sm/3.jpg" class="img-fluid blur-up lazyload bg-img" alt="" style="display: none;">
                                        </li>
                                    </ul>
                                    <h6>+12 people react this post</h6>
                                </div>
                            </div>
                            <div class="like-panel">
                                <div class="left-emoji">
                                    <ul>
                                        <li>
                                            <img src="../assets/svg/emoji/040.svg" alt="smile">
                                        </li>
                                        <li>
                                            <img src="../assets/svg/emoji/113.svg" alt="heart">
                                        </li>
                                        <li>
                                            <img src="../assets/svg/emoji/027.svg" alt="cry">
                                        </li>
                                        <li>
                                            <img src="../assets/svg/emoji/033.svg" alt="angry">
                                        </li>
                                    </ul>
                                    <h6>+75</h6>
                                </div>
                                <div class="right-stats">
                                    <ul>
                                        <li>
                                            <h5>
                                                <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-message-square iw-16 ih-16"><path d="M21 15a2 2 0 0 1-2 2H7l-4 4V5a2 2 0 0 1 2-2h14a2 2 0 0 1 2 2z"></path></svg>
                                                <span>4565</span> comment
                                            </h5>
                                        </li>
                                        <li>
                                            <h5>
                                                <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-share iw-16 ih-16"><path d="M4 12v8a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2v-8"></path><polyline points="16 6 12 2 8 6"></polyline><line x1="12" y1="2" x2="12" y2="15"></line></svg><span>985</span>
                                                share
                                            </h5>
                                        </li>
                                    </ul>
                                </div>
                            </div>
                            <div class="post-react">
                                <ul>
                                    <li class="react-btn">
                                        <a class="react-click" href="javascript:void(0)">
                                            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-smile iw-18 ih-18"><circle cx="12" cy="12" r="10"></circle><path d="M8 14s1.5 2 4 2 4-2 4-2"></path><line x1="9" y1="9" x2="9.01" y2="9"></line><line x1="15" y1="9" x2="15.01" y2="9"></line></svg> react
                                        </a>
                                        <div class="react-box">
                                            <ul>
                                                <li data-title="smile">
                                                    <a href="javascript:void(0)">
                                                        <img src="../assets/svg/emoji/040.svg" alt="smile">
                                                    </a>
                                                </li>
                                                <li data-title="love">
                                                    <a href="javascript:void(0)">
                                                        <img src="../assets/svg/emoji/113.svg" alt="heart">
                                                    </a>
                                                </li>
                                                <li data-title="cry">
                                                    <a href="javascript:void(0)">
                                                        <img src="../assets/svg/emoji/027.svg" alt="cry">
                                                    </a>
                                                </li>
                                                <li data-title="wow">
                                                    <a href="javascript:void(0)">
                                                        <img src="../assets/svg/emoji/052.svg" alt="angry">
                                                    </a>
                                                </li>
                                                <li data-title="angry">
                                                    <a href="javascript:void(0)">
                                                        <img src="../assets/svg/emoji/039.svg" alt="angry">
                                                    </a>
                                                </li>
                                                <li data-title="haha">
                                                    <a href="javascript:void(0)">
                                                        <img src="../assets/svg/emoji/042.svg" alt="">
                                                    </a>
                                                </li>
                                            </ul>
                                        </div>
                                    </li>
                                    <li class="comment-click">
                                        <a href="javascript:void(0)">
                                            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-message-square iw-18 ih-18"><path d="M21 15a2 2 0 0 1-2 2H7l-4 4V5a2 2 0 0 1 2-2h14a2 2 0 0 1 2 2z"></path></svg> comment
                                        </a>
                                    </li>
                                    <li data-bs-target="#shareModal" data-bs-toggle="modal">
                                        <a href="javascript:void(0)">
                                            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-share iw-16 ih-16"><path d="M4 12v8a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2v-8"></path><polyline points="16 6 12 2 8 6"></polyline><line x1="12" y1="2" x2="12" y2="15"></line></svg> share
                                        </a>
                                    </li>
                                </ul>
                            </div>
                            <div class="comment-section">
                                <div class="comments d-none">
                                    <div class="ldr-comments">
                                        <ul>
                                            <li>
                                                <div class="media">
                                                    <div class="ldr-img"></div>
                                                    <div class="media-body">
                                                        <div class="contents">
                                                            <div class="ldr-content"></div>
                                                            <div class="ldr-content"></div>
                                                        </div>
                                                    </div>
                                                </div>
                                                <ul class="sub-comment">
                                                    <li>
                                                        <div class="media">
                                                            <div class="ldr-img"></div>
                                                            <div class="media-body">
                                                                <div class="contents">
                                                                    <div class="ldr-content"></div>
                                                                    <div class="ldr-content"></div>
                                                                </div>
                                                            </div>
                                                        </div>
                                                    </li>
                                                </ul>
                                            </li>
                                            <li>
                                                <div class="media">
                                                    <div class="ldr-img"></div>
                                                    <div class="media-body">
                                                        <div class="contents">
                                                            <div class="ldr-content"></div>
                                                            <div class="ldr-content"></div>
                                                        </div>
                                                    </div>
                                                </div>
                                            </li>
                                            <li>
                                                <div class="media">
                                                    <div class="ldr-img"></div>
                                                    <div class="media-body">
                                                        <div class="contents">
                                                            <div class="ldr-content"></div>
                                                            <div class="ldr-content"></div>
                                                        </div>
                                                    </div>
                                                </div>
                                            </li>
                                        </ul>
                                    </div>
                                    <div class="main-comment">
                                        <div class="media">
                                            <a href="#" class="user-img bg-size blur-up lazyload" style="background-image: url(&quot;../assets/images/user-sm/2.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                                                <img src="../assets/images/user-sm/2.jpg" class="img-fluid blur-up lazyload bg-img" alt="user" style="display: none;">
                                            </a>
                                            <div class="media-body">
                                                <a href="#">
                                                    <h5>Pabelo Mukrani</h5>
                                                </a>
                                                <p>Oooo Very Cute and Sweet Dog, happy birthday Cuty....
                                                    🙂
                                                </p>
                                                <ul class="comment-option">
                                                    <li><a href="#">like (5)</a></li>
                                                    <li><a href="#">reply</a></li>
                                                    <li><a href="#">translate</a></li>
                                                </ul>
                                            </div>
                                            <div class="comment-time">
                                                <h6>50 mins ago</h6>
                                            </div>
                                        </div>
                                        <div class="sub-comment">
                                            <div class="media">
                                                <a href="#" class="user-img bg-size blur-up lazyload" style="background-image: url(&quot;../assets/images/user-sm/3.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                                                    <img src="../assets/images/user-sm/3.jpg" class="img-fluid blur-up lazyload bg-img" alt="user" style="display: none;">
                                                </a>
                                                <div class="media-body">
                                                    <a href="#">
                                                        <h5>sufiya elija</h5>
                                                    </a>
                                                    <p>Thank You So Much ❤❤</p>
                                                    <ul class="comment-option">
                                                        <li><a href="#">like</a></li>
                                                        <li><a href="#">reply</a></li>
                                                        <li><a href="#">translate</a></li>
                                                    </ul>
                                                </div>
                                                <div class="comment-time">
                                                    <h6>50 mins ago</h6>
                                                </div>
                                            </div>
                                            <div class="media">
                                                <a href="#" class="user-img bg-size blur-up lazyload" style="background-image: url(&quot;../assets/images/user-sm/4.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                                                    <img src="../assets/images/user-sm/4.jpg" class="img-fluid blur-up lazyload bg-img" alt="user" style="display: none;">
                                                </a>
                                                <div class="media-body">
                                                    <a href="#">
                                                        <h5>sufiya elija</h5>
                                                    </a>
                                                    <p>Thank You So Much ❤❤</p>
                                                    <ul class="comment-option">
                                                        <li><a href="#">like</a></li>
                                                        <li><a href="#">reply</a></li>
                                                        <li><a href="#">translate</a></li>
                                                    </ul>
                                                </div>
                                                <div class="comment-time">
                                                    <h6>50 mins ago</h6>
                                                </div>
                                            </div>
                                            <a href="javascript:void(0)" class="loader">
                                                <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-rotate-cw iw-15 ih-15"><polyline points="23 4 23 10 17 10"></polyline><path d="M20.49 15a9 9 0 1 1-2.12-9.36L23 10"></path></svg> load more
                                                replies
                                            </a>
                                        </div>
                                    </div>
                                    <div class="main-comment">
                                        <div class="media">
                                            <a href="#" class="user-img bg-size blur-up lazyload" style="background-image: url(&quot;../assets/images/user-sm/2.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                                                <img src="../assets/images/user-sm/2.jpg" class="img-fluid blur-up lazyload bg-img" alt="user" style="display: none;">
                                            </a>
                                            <div class="media-body">
                                                <a href="#">
                                                    <h5>Pabelo Mukrani</h5>
                                                </a>
                                                <p>It’s party time, Sufiya..... and happy birthday cuty 🎉🎊</p>
                                                <ul class="comment-option">
                                                    <li><a href="#">like</a></li>
                                                    <li><a href="#">reply</a></li>
                                                    <li><a href="#">translate</a></li>
                                                </ul>
                                            </div>
                                            <div class="comment-time">
                                                <h6>50 mins ago</h6>
                                            </div>
                                        </div>
                                    </div>
                                </div>
                                <div class="reply">
                                    <div class="search-input input-style input-lg icon-right">
                                        <input type="text" class="form-control emojiPicker" placeholder="write a comment..">
                                        <a href="javascript:void(0)">
                                            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-smile icon icon-2 iw-14 ih-14"><circle cx="12" cy="12" r="10"></circle><path d="M8 14s1.5 2 4 2 4-2 4-2"></path><line x1="9" y1="9" x2="9.01" y2="9"></line><line x1="15" y1="9" x2="15.01" y2="9"></line></svg>
                                        </a>
                                        <a href="javascript:void(0)">
                                            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-camera icon iw-14 ih-14"><path d="M23 19a2 2 0 0 1-2 2H3a2 2 0 0 1-2-2V8a2 2 0 0 1 2-2h4l2-3h6l2 3h4a2 2 0 0 1 2 2z"></path><circle cx="12" cy="13" r="4"></circle></svg>
                                        </a>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
                <div id="load-more" class="post-loader">
                    <div class="loader-icon">
                        <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-rotate-ccw icon-theme iw-25 ih-25"><polyline points="1 4 1 10 7 10"></polyline><path d="M3.51 15a9 9 0 1 0 2.13-9.36L1 10"></path></svg>
                    </div>
                    <div class="no-more-text">
                        <p>no more post</p>
                    </div>
                </div>
            </div>
            <div class="content-right d-xl-block d-none">
                <!-- birthday reminder -->
                <div class="birthday-section event-sec bg-size blur-up lazyloaded" style="background-image: url(&quot;../assets/images/event-bg.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                    <img src="../assets/images/event-bg.jpg" class="img-fluid blur-up lazyload bg-img" alt="birthday" style="display: none;">
                    <div class="birthday-top">
                        <div class="title">
                            <h3>college meet</h3>
                            <h6>today your collge group meeting</h6>
                        </div>
                        <div class="setting">
                            <div class="setting-btn light-btn">
                                <a href="#" class="d-flex">
                                    <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-rotate-cw iw-11 ih-11 icon icon-light stroke-width-3"><polyline points="23 4 23 10 17 10"></polyline><path d="M20.49 15a9 9 0 1 1-2.12-9.36L23 10"></path></svg>
                                </a>
                            </div>
                            <div class="setting-btn light-btn ms-2 setting-dropdown">
                                <div class=" btn-group custom-dropdown arrow-none dropdown-sm">
                                    <a class="d-flex" href="#" data-bs-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
                                        <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-sun icon-light stroke-width-3 iw-12 ih-12"><circle cx="12" cy="12" r="5"></circle><line x1="12" y1="1" x2="12" y2="3"></line><line x1="12" y1="21" x2="12" y2="23"></line><line x1="4.22" y1="4.22" x2="5.64" y2="5.64"></line><line x1="18.36" y1="18.36" x2="19.78" y2="19.78"></line><line x1="1" y1="12" x2="3" y2="12"></line><line x1="21" y1="12" x2="23" y2="12"></line><line x1="4.22" y1="19.78" x2="5.64" y2="18.36"></line><line x1="18.36" y1="5.64" x2="19.78" y2="4.22"></line></svg>
                                    </a>
                                    <div class="dropdown-menu dropdown-menu-right custom-dropdown">
                                        <ul>
                                            <li>
                                                <a href=""><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-edit icon-font-light iw-16 ih-16"><path d="M11 4H4a2 2 0 0 0-2 2v14a2 2 0 0 0 2 2h14a2 2 0 0 0 2-2v-7"></path><path d="M18.5 2.5a2.121 2.121 0 0 1 3 3L12 15l-4 1 1-4 9.5-9.5z"></path></svg>edit profile</a>
                                            </li>
                                            <li>
                                                <a href=""><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-user icon-font-light iw-16 ih-16"><path d="M20 21v-2a4 4 0 0 0-4-4H8a4 4 0 0 0-4 4v2"></path><circle cx="12" cy="7" r="4"></circle></svg>view profile</a>
                                            </li>
                                        </ul>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                    <div class="birthday-content">
                        <div class="image-section">
                            <div class="event-group">
                                <div class="center-profile bg-size blur-up lazyloaded" style="background-image: url(&quot;../assets/images/user-sm/3.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                                    <img src="../assets/images/user-sm/3.jpg" class="img-fluid blur-up lazyload bg-img" alt="user" style="display: none;">
                                </div>
                                <div class="center-profile bg-size blur-up lazyloaded" style="background-image: url(&quot;../assets/images/user-sm/5.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                                    <img src="../assets/images/user-sm/5.jpg" class="img-fluid blur-up lazyload bg-img" alt="user" style="display: none;">
                                </div>
                                <div class="center-profile bg-size blur-up lazyloaded" style="background-image: url(&quot;../assets/images/user-sm/2.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                                    <img src="../assets/images/user-sm/2.jpg" class="img-fluid blur-up lazyload bg-img" alt="user" style="display: none;">
                                </div>
                                <div class="center-profile bg-size blur-up lazyloaded" style="background-image: url(&quot;../assets/images/user-sm/1.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                                    <img src="../assets/images/user-sm/1.jpg" class="img-fluid blur-up lazyload bg-img" alt="user" style="display: none;">
                                </div>
                            </div>
                        </div>
                        <div class="details">
                            <h3><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-user icon-light me-2 stroke-width-3 iw-12 ih-12"><path d="M20 21v-2a4 4 0 0 0-4-4H8a4 4 0 0 0-4 4v2"></path><circle cx="12" cy="7" r="4"></circle></svg>56
                                people</h3>
                            <h6>glasgow, scotland</h6>
                            <p>Lorem 5th Sept 2019 dummy text of the printing and typesetting industry.</p>
                            <form>
                                <input type="text" placeholder="send invitation" class="form-control">
                                <button type="submit">
                                    <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-arrow-right iw-13 ih-13 icon-light icon stroke-width-3"><line x1="5" y1="12" x2="19" y2="12"></line><polyline points="12 5 19 12 12 19"></polyline></svg>
                                </button>
                            </form>
                        </div>
                    </div>
                </div>

                <!-- gallery section -->
                <div class="gallery-section section-t-space">
                    <div class="gallery-top">
                        <div class="card-title">
                            <h3>gallery</h3>
                            <h5>156 photos</h5>
                            <div class="settings">
                                <div class="setting-btn">
                                    <a href="#">
                                        <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-rotate-cw icon icon-dark stroke-width-3 iw-11 ih-11"><polyline points="23 4 23 10 17 10"></polyline><path d="M20.49 15a9 9 0 1 1-2.12-9.36L23 10"></path></svg>
                                    </a>
                                </div>
                                <div class="setting-btn ms-2 setting-dropdown">
                                    <div class="btn-group custom-dropdown arrow-none dropdown-sm">
                                        <a href="#" data-bs-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
                                            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-sun icon-dark stroke-width-3 icon iw-11 ih-11"><circle cx="12" cy="12" r="5"></circle><line x1="12" y1="1" x2="12" y2="3"></line><line x1="12" y1="21" x2="12" y2="23"></line><line x1="4.22" y1="4.22" x2="5.64" y2="5.64"></line><line x1="18.36" y1="18.36" x2="19.78" y2="19.78"></line><line x1="1" y1="12" x2="3" y2="12"></line><line x1="21" y1="12" x2="23" y2="12"></line><line x1="4.22" y1="19.78" x2="5.64" y2="18.36"></line><line x1="18.36" y1="5.64" x2="19.78" y2="4.22"></line></svg>
                                        </a>
                                        <div class="dropdown-menu dropdown-menu-right custom-dropdown">
                                            <ul>
                                                <li>
                                                    <a href=""><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-edit icon-font-light iw-16 ih-16"><path d="M11 4H4a2 2 0 0 0-2 2v14a2 2 0 0 0 2 2h14a2 2 0 0 0 2-2v-7"></path><path d="M18.5 2.5a2.121 2.121 0 0 1 3 3L12 15l-4 1 1-4 9.5-9.5z"></path></svg>edit
                                                        profile</a>
                                                </li>
                                                <li>
                                                    <a href=""><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-user icon-font-light iw-16 ih-16"><path d="M20 21v-2a4 4 0 0 0-4-4H8a4 4 0 0 0-4 4v2"></path><circle cx="12" cy="7" r="4"></circle></svg>view
                                                        profile</a>
                                                </li>
                                            </ul>
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                    <div class="portfolio-section ratio_square">
                        <div class="container-fluid p-0">
                            <div class="row">
                                <div class="col-4">
                                    <div class="overlay">
                                        <div class="portfolio-image">
                                            <a href="javascript:void(0)" data-bs-toggle="modal" data-bs-target="#imageModel" class="bg-size blur-up lazyloaded" style="background-image: url(&quot;../assets/images/story/1.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                                                <img src="../assets/images/story/1.jpg" alt="" class="img-fluid blur-up lazyload bg-img" style="display: none;">
                                            </a>
                                        </div>
                                    </div>
                                </div>
                                <div class="col-4">
                                    <div class="overlay">
                                        <div class="portfolio-image">
                                            <a href="javascript:void(0)" data-bs-toggle="modal" data-bs-target="#imageModel" class="bg-size blur-up lazyloaded" style="background-image: url(&quot;../assets/images/story/2.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                                                <img src="../assets/images/story/2.jpg" alt="" class="img-fluid blur-up lazyload bg-img" style="display: none;">
                                            </a>
                                        </div>
                                    </div>
                                </div>
                                <div class="col-4">
                                    <div class="overlay">
                                        <div class="portfolio-image">
                                            <a href="javascript:void(0)" data-bs-toggle="modal" data-bs-target="#imageModel" class="bg-size blur-up lazyloaded" style="background-image: url(&quot;../assets/images/story/3.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                                                <img src="../assets/images/story/3.jpg" alt="" class="img-fluid blur-up lazyload bg-img" style="display: none;">
                                            </a>
                                        </div>
                                    </div>
                                </div>
                                <div class="col-4 row m-0">
                                    <div class="col-12 pt-cls p-0">
                                        <div class="overlay">
                                            <div class="portfolio-image">
                                                <a href="javascript:void(0)" data-bs-toggle="modal" data-bs-target="#imageModel" class="bg-size blur-up lazyloaded" style="background-image: url(&quot;../assets/images/story/4.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                                                    <img src="../assets/images/story/4.jpg" alt="" class="img-fluid blur-up lazyload bg-img" style="display: none;">
                                                </a>
                                            </div>
                                        </div>
                                    </div>
                                    <div class="col-12 pt-cls p-0">
                                        <div class="overlay">
                                            <div class="portfolio-image">
                                                <a href="javascript:void(0)" data-bs-toggle="modal" data-bs-target="#imageModel" class="bg-size blur-up lazyloaded" style="background-image: url(&quot;../assets/images/story/6.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                                                    <img src="../assets/images/story/6.jpg" alt="" class="img-fluid blur-up lazyload bg-img" style="display: none;">
                                                </a>
                                            </div>
                                        </div>
                                    </div>
                                </div>
                                <div class="col-8 pt-cls">
                                    <div class="overlay">
                                        <div class="portfolio-image">
                                            <a href="javascript:void(0)" data-bs-toggle="modal" data-bs-target="#imageModel" class="bg-size blur-up lazyloaded" style="background-image: url(&quot;../assets/images/story/5.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                                                <img src="../assets/images/story/5.jpg" alt="" class="img-fluid blur-up lazyload bg-img" style="display: none;">
                                            </a>
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
                <!-- acitivity feed -->
                <div class="activity-list section-t-space">
                    <div class="card-title">
                        <h3>activity feed</h3>
                        <div class="settings">
                            <div class="setting-btn">
                                <a href="#" class="d-flex">
                                    <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-rotate-cw icon icon-theme stroke-width-3 iw-11 ih-11"><polyline points="23 4 23 10 17 10"></polyline><path d="M20.49 15a9 9 0 1 1-2.12-9.36L23 10"></path></svg>
                                </a>
                            </div>
                            <div class="setting-btn ms-2 setting-dropdown">
                                <div class=" btn-group custom-dropdown arrow-none dropdown-sm">
                                    <a href="#" data-bs-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
                                        <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-sun icon-dark stroke-width-3 icon iw-11 ih-11"><circle cx="12" cy="12" r="5"></circle><line x1="12" y1="1" x2="12" y2="3"></line><line x1="12" y1="21" x2="12" y2="23"></line><line x1="4.22" y1="4.22" x2="5.64" y2="5.64"></line><line x1="18.36" y1="18.36" x2="19.78" y2="19.78"></line><line x1="1" y1="12" x2="3" y2="12"></line><line x1="21" y1="12" x2="23" y2="12"></line><line x1="4.22" y1="19.78" x2="5.64" y2="18.36"></line><line x1="18.36" y1="5.64" x2="19.78" y2="4.22"></line></svg>
                                    </a>
                                    <div class="dropdown-menu dropdown-menu-right custom-dropdown">
                                        <ul>
                                            <li>
                                                <a href=""><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-edit icon-font-light iw-16 ih-16"><path d="M11 4H4a2 2 0 0 0-2 2v14a2 2 0 0 0 2 2h14a2 2 0 0 0 2-2v-7"></path><path d="M18.5 2.5a2.121 2.121 0 0 1 3 3L12 15l-4 1 1-4 9.5-9.5z"></path></svg>see all</a>
                                            </li>
                                            <li>
                                                <a href=""><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-search icon-font-light iw-16 ih-16"><circle cx="11" cy="11" r="8"></circle><line x1="21" y1="21" x2="16.65" y2="16.65"></line></svg>find page</a>
                                            </li>
                                            <li>
                                                <a href=""><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-settings icon-font-light iw-16 ih-16"><circle cx="12" cy="12" r="3"></circle><path d="M19.4 15a1.65 1.65 0 0 0 .33 1.82l.06.06a2 2 0 0 1 0 2.83 2 2 0 0 1-2.83 0l-.06-.06a1.65 1.65 0 0 0-1.82-.33 1.65 1.65 0 0 0-1 1.51V21a2 2 0 0 1-2 2 2 2 0 0 1-2-2v-.09A1.65 1.65 0 0 0 9 19.4a1.65 1.65 0 0 0-1.82.33l-.06.06a2 2 0 0 1-2.83 0 2 2 0 0 1 0-2.83l.06-.06a1.65 1.65 0 0 0 .33-1.82 1.65 1.65 0 0 0-1.51-1H3a2 2 0 0 1-2-2 2 2 0 0 1 2-2h.09A1.65 1.65 0 0 0 4.6 9a1.65 1.65 0 0 0-.33-1.82l-.06-.06a2 2 0 0 1 0-2.83 2 2 0 0 1 2.83 0l.06.06a1.65 1.65 0 0 0 1.82.33H9a1.65 1.65 0 0 0 1-1.51V3a2 2 0 0 1 2-2 2 2 0 0 1 2 2v.09a1.65 1.65 0 0 0 1 1.51 1.65 1.65 0 0 0 1.82-.33l.06-.06a2 2 0 0 1 2.83 0 2 2 0 0 1 0 2.83l-.06.06a1.65 1.65 0 0 0-.33 1.82V9a1.65 1.65 0 0 0 1.51 1H21a2 2 0 0 1 2 2 2 2 0 0 1-2 2h-.09a1.65 1.65 0 0 0-1.51 1z"></path></svg>settings</a>
                                            </li>
                                        </ul>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                    <div class="activity-content">
                        <ul>
                            <li>
                                <div class="media">
                                    <div class="img-part bg-size blur-up lazyloaded" style="background-image: url(&quot;../assets/images/user-sm/1.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                                        <img src="../assets/images/user-sm/1.jpg" class="img-fluid blur-up lazyload bg-img" alt="" style="display: none;">
                                    </div>
                                    <div class="media-body">
                                        <h4>Bill Yerds commented on <span>Anna sthesia's</span> photo</h4>
                                        <h6>5 mins ago</h6>
                                    </div>
                                </div>
                            </li>
                            <li>
                                <div class="media">
                                    <div class="img-part bg-size blur-up lazyloaded" style="background-image: url(&quot;../assets/images/user-sm/2.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                                        <img src="../assets/images/user-sm/2.jpg" class="img-fluid blur-up lazyload bg-img" alt="" style="display: none;">
                                    </div>
                                    <div class="media-body">
                                        <h4>Bill Yerds liked <span>Paige Turner's</span> photo</h4>
                                        <h6>15 mins ago</h6>
                                    </div>
                                </div>
                            </li>
                            <li>
                                <div class="media">
                                    <div class="img-part bg-size blur-up lazyloaded" style="background-image: url(&quot;../assets/images/user-sm/3.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                                        <img src="../assets/images/user-sm/3.jpg" class="img-fluid blur-up lazyload bg-img" alt="" style="display: none;">
                                    </div>
                                    <div class="media-body">
                                        <h4>Bill Yerds reacted on <span>Paul Molive's</span> photo</h4>
                                        <h6>1 day ago</h6>
                                    </div>
                                </div>
                            </li>
                            <li>
                                <div class="media">
                                    <div class="img-part bg-size blur-up lazyload" style="background-image: url(&quot;../assets/images/user-sm/4.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                                        <img src="../assets/images/user-sm/4.jpg" class="img-fluid blur-up lazyload bg-img" alt="" style="display: none;">
                                    </div>
                                    <div class="media-body">
                                        <h4>Bill Yerds commented on <span>Anna Mull's</span> photo</h4>
                                        <h6>1 day ago</h6>
                                    </div>
                                </div>
                            </li>
                            <li>
                                <div class="media">
                                    <div class="img-part bg-size blur-up lazyload" style="background-image: url(&quot;../assets/images/user-sm/5.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                                        <img src="../assets/images/user-sm/5.jpg" class="img-fluid blur-up lazyload bg-img" alt="" style="display: none;">
                                    </div>
                                    <div class="media-body">
                                        <h4>Bill Yerds commented on <span>Anna sthesia's</span> photo</h4>
                                        <h6>2 day ago</h6>
                                    </div>
                                </div>
                            </li>
                        </ul>
                    </div>
                </div>
                <div class="sticky-top">
                    <!-- event -->
                    <div class="event-box section-t-space ratio2_3">
                        <div class="image-section bg-size blur-up lazyload" style="background-image: url(&quot;../assets/images/post/12.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                            <img src="../assets/images/post/12.jpg" class="img-fluid blur-up lazyload bg-img" alt="event" style="display: none;">
                            <div class="card-title">
                                <h3>event</h3>
                                <div class="settings">
                                    <div class="setting-btn">
                                        <a href="#" class="d-flex">
                                            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-rotate-cw icon icon-dark stroke-width-3 iw-11 ih-11"><polyline points="23 4 23 10 17 10"></polyline><path d="M20.49 15a9 9 0 1 1-2.12-9.36L23 10"></path></svg>
                                        </a>
                                    </div>
                                    <div class="setting-btn ms-2 setting-dropdown">
                                        <div class=" btn-group custom-dropdown arrow-none dropdown-sm">
                                            <a href="#" data-bs-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
                                                <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-sun icon-dark stroke-width-3 icon iw-11 ih-11"><circle cx="12" cy="12" r="5"></circle><line x1="12" y1="1" x2="12" y2="3"></line><line x1="12" y1="21" x2="12" y2="23"></line><line x1="4.22" y1="4.22" x2="5.64" y2="5.64"></line><line x1="18.36" y1="18.36" x2="19.78" y2="19.78"></line><line x1="1" y1="12" x2="3" y2="12"></line><line x1="21" y1="12" x2="23" y2="12"></line><line x1="4.22" y1="19.78" x2="5.64" y2="18.36"></line><line x1="18.36" y1="5.64" x2="19.78" y2="4.22"></line></svg>
                                            </a>
                                            <div class="dropdown-menu dropdown-menu-right custom-dropdown">
                                                <ul>
                                                    <li>
                                                        <a href=""><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-edit icon-font-light iw-16 ih-16"><path d="M11 4H4a2 2 0 0 0-2 2v14a2 2 0 0 0 2 2h14a2 2 0 0 0 2-2v-7"></path><path d="M18.5 2.5a2.121 2.121 0 0 1 3 3L12 15l-4 1 1-4 9.5-9.5z"></path></svg>remind
                                                            me</a>
                                                    </li>
                                                    <li>
                                                        <a href=""><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-settings icon-font-light iw-16 ih-16"><circle cx="12" cy="12" r="3"></circle><path d="M19.4 15a1.65 1.65 0 0 0 .33 1.82l.06.06a2 2 0 0 1 0 2.83 2 2 0 0 1-2.83 0l-.06-.06a1.65 1.65 0 0 0-1.82-.33 1.65 1.65 0 0 0-1 1.51V21a2 2 0 0 1-2 2 2 2 0 0 1-2-2v-.09A1.65 1.65 0 0 0 9 19.4a1.65 1.65 0 0 0-1.82.33l-.06.06a2 2 0 0 1-2.83 0 2 2 0 0 1 0-2.83l.06-.06a1.65 1.65 0 0 0 .33-1.82 1.65 1.65 0 0 0-1.51-1H3a2 2 0 0 1-2-2 2 2 0 0 1 2-2h.09A1.65 1.65 0 0 0 4.6 9a1.65 1.65 0 0 0-.33-1.82l-.06-.06a2 2 0 0 1 0-2.83 2 2 0 0 1 2.83 0l.06.06a1.65 1.65 0 0 0 1.82.33H9a1.65 1.65 0 0 0 1-1.51V3a2 2 0 0 1 2-2 2 2 0 0 1 2 2v.09a1.65 1.65 0 0 0 1 1.51 1.65 1.65 0 0 0 1.82-.33l.06-.06a2 2 0 0 1 2.83 0 2 2 0 0 1 0 2.83l-.06.06a1.65 1.65 0 0 0-.33 1.82V9a1.65 1.65 0 0 0 1.51 1H21a2 2 0 0 1 2 2 2 2 0 0 1-2 2h-.09a1.65 1.65 0 0 0-1.51 1z"></path></svg>setting</a>
                                                    </li>
                                                </ul>
                                            </div>
                                        </div>
                                    </div>
                                </div>
                            </div>
                            <div class="play-btn" data-bs-toggle="modal" data-bs-target="#videoPlayer">
                                <img src="../assets/images/icon/play.png" class="img-fluid blur-up lazyload" alt="play">
                            </div>
                        </div>
                        <div class="event-content">
                            <h3>happy life event</h3>
                            <h6>26 january 2021</h6>
                            <p>Lorem Ipsum is simply dummy text of the printing and typesetting industry
                                <span>15256 People Going</span></p>
                            <div class="bottom-part">
                                <a href="#" class="event-btn">interested / not in..</a>
                            </div>
                            <a href="#" class="share-btn">
                                <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-corner-up-right icon-dark stroke-width-3 iw-14 ih-14"><polyline points="15 14 20 9 15 4"></polyline><path d="M4 20v-7a4 4 0 0 1 4-4h12"></path></svg>
                            </a>
                        </div>
                    </div>

                    <!-- hashtag-list box -->
                    <div class="hashtag-list section-t-space">
                        <div class="card-title">
                            <h3>#worldwide trends</h3>
                            <div class="settings">
                                <div class="setting-btn">
                                    <a href="#" class="d-flex">
                                        <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-rotate-cw icon icon-dark stroke-width-3 iw-11 ih-11"><polyline points="23 4 23 10 17 10"></polyline><path d="M20.49 15a9 9 0 1 1-2.12-9.36L23 10"></path></svg>
                                    </a>
                                </div>
                                <div class="setting-btn ms-2 setting-dropdown">
                                    <div class=" btn-group custom-dropdown arrow-none dropdown-sm">
                                        <a href="#" data-bs-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
                                            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-sun icon-dark stroke-width-3 icon iw-11 ih-11"><circle cx="12" cy="12" r="5"></circle><line x1="12" y1="1" x2="12" y2="3"></line><line x1="12" y1="21" x2="12" y2="23"></line><line x1="4.22" y1="4.22" x2="5.64" y2="5.64"></line><line x1="18.36" y1="18.36" x2="19.78" y2="19.78"></line><line x1="1" y1="12" x2="3" y2="12"></line><line x1="21" y1="12" x2="23" y2="12"></line><line x1="4.22" y1="19.78" x2="5.64" y2="18.36"></line><line x1="18.36" y1="5.64" x2="19.78" y2="4.22"></line></svg>
                                        </a>
                                        <div class="dropdown-menu dropdown-menu-right custom-dropdown">
                                            <ul>
                                                <li>
                                                    <a href=""><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-edit icon-font-light iw-16 ih-16"><path d="M11 4H4a2 2 0 0 0-2 2v14a2 2 0 0 0 2 2h14a2 2 0 0 0 2-2v-7"></path><path d="M18.5 2.5a2.121 2.121 0 0 1 3 3L12 15l-4 1 1-4 9.5-9.5z"></path></svg>see all</a>
                                                </li>
                                                <li>
                                                    <a href=""><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-search icon-font-light iw-16 ih-16"><circle cx="11" cy="11" r="8"></circle><line x1="21" y1="21" x2="16.65" y2="16.65"></line></svg>find
                                                        page</a>
                                                </li>
                                                <li>
                                                    <a href=""><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-settings icon-font-light iw-16 ih-16"><circle cx="12" cy="12" r="3"></circle><path d="M19.4 15a1.65 1.65 0 0 0 .33 1.82l.06.06a2 2 0 0 1 0 2.83 2 2 0 0 1-2.83 0l-.06-.06a1.65 1.65 0 0 0-1.82-.33 1.65 1.65 0 0 0-1 1.51V21a2 2 0 0 1-2 2 2 2 0 0 1-2-2v-.09A1.65 1.65 0 0 0 9 19.4a1.65 1.65 0 0 0-1.82.33l-.06.06a2 2 0 0 1-2.83 0 2 2 0 0 1 0-2.83l.06-.06a1.65 1.65 0 0 0 .33-1.82 1.65 1.65 0 0 0-1.51-1H3a2 2 0 0 1-2-2 2 2 0 0 1 2-2h.09A1.65 1.65 0 0 0 4.6 9a1.65 1.65 0 0 0-.33-1.82l-.06-.06a2 2 0 0 1 0-2.83 2 2 0 0 1 2.83 0l.06.06a1.65 1.65 0 0 0 1.82.33H9a1.65 1.65 0 0 0 1-1.51V3a2 2 0 0 1 2-2 2 2 0 0 1 2 2v.09a1.65 1.65 0 0 0 1 1.51 1.65 1.65 0 0 0 1.82-.33l.06-.06a2 2 0 0 1 2.83 0 2 2 0 0 1 0 2.83l-.06.06a1.65 1.65 0 0 0-.33 1.82V9a1.65 1.65 0 0 0 1.51 1H21a2 2 0 0 1 2 2 2 2 0 0 1-2 2h-.09a1.65 1.65 0 0 0-1.51 1z"></path></svg>settings</a>
                                                </li>
                                            </ul>
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                        <div class="hashtag-content">
                            <ul>
                                <li>
                                    <a href="#">
                                        <h5>#CitizenshipAmendmentBill2019</h5>
                                    </a>
                                    <h6><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-mail iw-11 ih-11"><path d="M4 4h16c1.1 0 2 .9 2 2v12c0 1.1-.9 2-2 2H4c-1.1 0-2-.9-2-2V6c0-1.1.9-2 2-2z"></path><polyline points="22,6 12,13 2,6"></polyline></svg> 15k post</h6>
                                </li>
                                <li>
                                    <a href="#">
                                        <h5>#BestFriend</h5>
                                    </a>
                                    <h6><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-mail iw-11 ih-11"><path d="M4 4h16c1.1 0 2 .9 2 2v12c0 1.1-.9 2-2 2H4c-1.1 0-2-.9-2-2V6c0-1.1.9-2 2-2z"></path><polyline points="22,6 12,13 2,6"></polyline></svg> 574k post</h6>
                                </li>
                                <li>
                                    <a href="#">
                                        <h5>#loveYourSelf</h5>
                                    </a>
                                    <h6><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-mail iw-11 ih-11"><path d="M4 4h16c1.1 0 2 .9 2 2v12c0 1.1-.9 2-2 2H4c-1.1 0-2-.9-2-2V6c0-1.1.9-2 2-2z"></path><polyline points="22,6 12,13 2,6"></polyline></svg> 125k post</h6>
                                </li>
                                <li>
                                    <a href="#">
                                        <h5>#planWalkEvent</h5>
                                    </a>
                                    <h6><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-mail iw-11 ih-11"><path d="M4 4h16c1.1 0 2 .9 2 2v12c0 1.1-.9 2-2 2H4c-1.1 0-2-.9-2-2V6c0-1.1.9-2 2-2z"></path><polyline points="22,6 12,13 2,6"></polyline></svg> 105k post</h6>
                                </li>
                            </ul>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>

</div>