<script>
// @ts-nocheck

  import Storybox from "$lib/storybox.svelte";
  import CreatePost from "$lib/component/createPost.svelte" 
  import { onMount } from "svelte";

  let _ = (el) => document.querySelectorAll(el);
  onMount(
    () => {
        _("img.lazyload").forEach((node) => {
            node.classList.remove("blur-up")
        })

        _(".bg-img").forEach((node)=>{
           let src = node.getAttribute('src');
            console.log(src);
           let parent = node.parentElement;


            parent.setAttribute("style", `background-image: url('`+ src + `');background-size:cover;
            background-position: center; background-repeat: no-repeat;display: block`)

            node.remove();
        })
    }
  )
</script>
<Storybox />

<div class="container-fluid section-t-space px-0 layout-default">
    <div class="page-content">
        <div class="content-left">
            <!-- profile box -->
            <div class="profile-box">
                <div class="profile-setting">
                    <div class="setting-btn refresh">
                        <a href=/# class="d-flex">
                            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-rotate-cw icon icon-theme stroke-width-3 iw-11 ih-11"><polyline points="23 4 23 10 17 10"></polyline><path d="M20.49 15a9 9 0 1 1-2.12-9.36L23 10"></path></svg>
                        </a>
                    </div>
                    <div class="setting-btn setting setting-dropdown">
                        <div class="btn-group custom-dropdown arrow-none dropdown-sm">
                            <a href=/# class="d-flex" data-bs-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
                                <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-sun icon icon-theme stroke-width-3 iw-11 ih-11"><circle cx="12" cy="12" r="5"></circle><line x1="12" y1="1" x2="12" y2="3"></line><line x1="12" y1="21" x2="12" y2="23"></line><line x1="4.22" y1="4.22" x2="5.64" y2="5.64"></line><line x1="18.36" y1="18.36" x2="19.78" y2="19.78"></line><line x1="1" y1="12" x2="3" y2="12"></line><line x1="21" y1="12" x2="23" y2="12"></line><line x1="4.22" y1="19.78" x2="5.64" y2="18.36"></line><line x1="18.36" y1="5.64" x2="19.78" y2="4.22"></line></svg>
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
                <div class="profile-content">
                    <a href="profile.html" class="image-section">
                        <div class="profile-img">
                            <div class="bg-size blur-up lazyloaded" style="background-image: url(&quot;images/story/8.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                                <img src="images/story/8.jpg" class="img-fluid blur-up lazyload bg-img" alt="profile" style="display: none;">
                            </div>
                            <span class="stats">
                                <img src="images/icon/verified.png" class="img-fluid blur-up lazyloaded" alt="verified">
                            </span>
                        </div>
                    </a>
                    <div class="profile-detail">
                        <a href="profile.html">
                            <h2>kelin jasen <span>❤</span></h2>
                        </a>
                        <h5>kelin.jasen156@gmail.com</h5>
                        <div class="description">
                            <p>Lorem Ipsum is simply dummy text of the printing and typesetting industry.
                            </p>
                        </div>
                        <div class="counter-stats">
                            <ul id="counter">
                                <li>
                                    <h3 class="counter-value" data-count="546">0</h3>
                                    <h5>following</h5>
                                </li>
                                <li>
                                    <h3 class="counter-value" data-count="26335">0</h3>
                                    <h5>likes</h5>
                                </li>
                                <li>
                                    <h3 class="counter-value" data-count="6845">0</h3>
                                    <h5>followers</h5>
                                </li>
                            </ul>
                        </div>
                        <a href=/# class="btn btn-solid">view profile</a>
                    </div>
                </div>
            </div>
            <!-- suggestion box -->
            <div class="suggestion-box section-t-space">
                <div class="card-title">
                    <h3>friend suggestion</h3>
                    <div class="settings">
                        <div class="setting-btn">
                            <a href=/# class="d-flex">
                                <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-rotate-cw icon icon-theme stroke-width-3 iw-11 ih-11"><polyline points="23 4 23 10 17 10"></polyline><path d="M20.49 15a9 9 0 1 1-2.12-9.36L23 10"></path></svg>
                            </a>
                        </div>
                        <div class="setting-btn setting-dropdown ms-2">
                            <div class="btn-group custom-dropdown arrow-none dropdown-sm">
                                <a href=/# class="d-flex" data-bs-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
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
                    <div class="slide-2 no-arrow default-space slick-initialized slick-slider"><button class="slick-prev slick-arrow" aria-label="Previous" type="button" aria-disabled="false" style="display: inline-block;">Previous</button><div class="slick-list draggable"><div class="slick-track" style="opacity: 1; width: 405px; transform: translate3d(-135px, 0px, 0px);"><div class="slick-slide" data-slick-index="0" aria-hidden="true" style="width: 135px;" tabindex="-1"><div><div style="width: 100%; display: inline-block;">
                            <div class="story-box">
                                <div class="adaptive-overlay pink-overlay"></div>
                                <div class="story-bg bg-size" style="background-image: url(&quot;images/story/2.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                                    <img src="images/story/2.jpg" class="img-fluid bg-img" data-adaptive-background="1" alt="" style="display: none;">
                                </div>
                                <div class="story-content">
                                    <h6>josephin water</h6>
                                    <span>active now</span>
                                </div>
                            </div>
                        </div></div></div><div class="slick-slide slick-current slick-active" data-slick-index="1" aria-hidden="false" style="width: 135px;"><div><div style="width: 100%; display: inline-block;">
                            <div class="story-box">
                                <div class="adaptive-overlay blue-overlay"></div>
                                <div class="story-bg bg-size" style="background-image: url(&quot;images/story/7.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                                    <img src="images/story/7.jpg" class="img-fluid bg-img" data-adaptive-background="1" alt="" style="display: none;">
                                </div>
                                <div class="story-content">
                                    <h6>josephin water</h6>
                                    <span>active now</span>
                                </div>
                            </div>
                        </div></div></div><div class="slick-slide slick-active" data-slick-index="2" aria-hidden="false" style="width: 135px;"><div><div style="width: 100%; display: inline-block;">
                            <div class="story-box">
                                <div class="adaptive-overlay skin-overlay"></div>
                                <div class="story-bg bg-size" style="background-image: url(&quot;images/story/1.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                                    <img src="images/story/1.jpg" class="img-fluid bg-img" data-adaptive-background="1" alt="" style="display: none;">
                                </div>
                                <div class="story-content">
                                    <h6>josephin water</h6>
                                    <span>active now</span>
                                </div>
                            </div>
                        </div></div></div></div></div><button class="slick-next slick-arrow slick-disabled" aria-label="Next" type="button" style="display: inline-block;" aria-disabled="true">Next</button></div>
                </div>
            </div>
            <div class="sticky-top">
                <!-- like page -->
                <div class="page-list section-t-space">
                    <div class="card-title">
                        <h3>liked pages</h3>
                        <h5>18 pages</h5>
                        <div class="settings">
                            <div class="setting-btn">
                                <a href=/# class="d-flex">
                                    <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-rotate-cw icon icon-dark stroke-width-3 iw-11 ih-11"><polyline points="23 4 23 10 17 10"></polyline><path d="M20.49 15a9 9 0 1 1-2.12-9.36L23 10"></path></svg>
                                </a>
                            </div>
                            <div class="setting-btn ms-2 setting-dropdown">
                                <div class="btn-group custom-dropdown arrow-none dropdown-sm">
                                    <a href=/# data-bs-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
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
                                    <div class="img-part bg-size blur-up lazyloaded" style="background-image: url(&quot;images/pages-logo/1.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                                        <img src="images/pages-logo/1.jpg" class="img-fluid blur-up lazyload bg-img" alt="" style="display: none;">
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
                                    <div class="img-part bg-size blur-up lazyloaded" style="background-image: url(&quot;images/pages-logo/2.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                                        <img src="images/pages-logo/2.jpg" class="img-fluid blur-up lazyload bg-img" alt="" style="display: none;">
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
                                    <div class="img-part bg-size blur-up lazyloaded" style="background-image: url(&quot;images/pages-logo/3.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                                        <img src="images/pages-logo/3.jpg" class="img-fluid blur-up lazyload bg-img" alt="" style="display: none;">
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
                                    <div class="img-part bg-size blur-up lazyloaded" style="background-image: url(&quot;images/pages-logo/4.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                                        <img src="images/pages-logo/4.jpg" class="img-fluid blur-up lazyload bg-img" alt="" style="display: none;">
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
                                    <div class="img-part bg-size blur-up lazyloaded" style="background-image: url(&quot;images/pages-logo/5.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                                        <img src="images/pages-logo/5.jpg" class="img-fluid blur-up lazyload bg-img" alt="" style="display: none;">
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
                <!-- weather section -->
                <div class="weather-section section-t-space">
                    <div class="card-title light-version">
                        <h3>weather</h3>
                        <div class="settings">
                            <div class="setting-btn light-btn">
                                <a href=/# class="d-flex">
                                    <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-rotate-cw icon icon-light stroke-width-3 iw-11 ih-11"><polyline points="23 4 23 10 17 10"></polyline><path d="M20.49 15a9 9 0 1 1-2.12-9.36L23 10"></path></svg>
                                </a>
                            </div>
                            <div class="setting-btn light-btn ms-2 setting-dropdown">
                                <div class="btn-group custom-dropdown arrow-none dropdown-sm">
                                    <a class="d-flex" href=/# data-bs-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
                                        <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-sun icon-light stroke-width-3 iw-12 ih-12"><circle cx="12" cy="12" r="5"></circle><line x1="12" y1="1" x2="12" y2="3"></line><line x1="12" y1="21" x2="12" y2="23"></line><line x1="4.22" y1="4.22" x2="5.64" y2="5.64"></line><line x1="18.36" y1="18.36" x2="19.78" y2="19.78"></line><line x1="1" y1="12" x2="3" y2="12"></line><line x1="21" y1="12" x2="23" y2="12"></line><line x1="4.22" y1="19.78" x2="5.64" y2="18.36"></line><line x1="18.36" y1="5.64" x2="19.78" y2="4.22"></line></svg>
                                    </a>
                                    <div class="dropdown-menu dropdown-menu-right custom-dropdown">
                                        <ul>
                                            <li>
                                                <a href=""><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-edit icon-font-light iw-16 ih-16"><path d="M11 4H4a2 2 0 0 0-2 2v14a2 2 0 0 0 2 2h14a2 2 0 0 0 2-2v-7"></path><path d="M18.5 2.5a2.121 2.121 0 0 1 3 3L12 15l-4 1 1-4 9.5-9.5z"></path></svg>change
                                                    city</a>
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
                    <div class="weather-content">
                        <div class="top-title">
                            <h2>28°C</h2>
                            <h5>4.45 pm</h5>
                        </div>
                        <h5>sunny day</h5>
                        <h6>21 march 2021 (monday) <span>denmark</span></h6>
                    </div>
                    <div class="flaks-img">
                        <img src="images/icon/snow-flaks.png" class="img-fluid blur-up lazyload" alt="snow">
                    </div>
                    <div class="snowflakes" aria-hidden="true">
                        <div class="snowflake">
                            ❅
                        </div>
                        <div class="snowflake">
                            ❆
                        </div>
                        <div class="snowflake">
                            ❅
                        </div>
                        <div class="snowflake">
                            ❆
                        </div>
                        <div class="snowflake">
                            ❅
                        </div>
                        <div class="snowflake">
                            ❆
                        </div>
                        <div class="snowflake">
                            ❅
                        </div>
                        <div class="snowflake">
                            ❆
                        </div>
                        <div class="snowflake">
                            ❅
                        </div>
                        <div class="snowflake">
                            ❆
                        </div>
                        <div class="snowflake">
                            ❅
                        </div>
                        <div class="snowflake">
                            ❆
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <div class="content-center">
            <CreatePost />
            <div class="overlay-bg"></div>
            <div class="post-panel infinite-loader-sec section-t-space">
                <div class="post-wrapper">
                    <div class="post-title">
                        <div class="profile">
                            <div class="media">
                                <a class="popover-cls user-img rounded-full" data-bs-toggle="popover" data-placement="right"
                                    data-name="sufiya eliza" data-img="images/user-sm/1.jpg">
                                    <img src="images/user-sm/1.jpg"
                                        class="img-fluid blur-up lazyload bg-img" alt="user">
                                </a>
                                <div class="media-body">
                                    <a href="#">
                                        <h5>sufiya eliza</h5>
                                    </a>
                                    <h6>30 mins ago</h6>
                                </div>
                            </div>
                        </div>
                        <div class="setting-btn ms-auto setting-dropdown no-bg">
                            <div class="btn-group custom-dropdown arrow-none dropdown-sm">
                                <div role="button" data-bs-toggle="dropdown" aria-haspopup="true"
                                    aria-expanded="false">
                                    <i class="icon icon-font-color iw-14"
                                        data-feather="more-horizontal"></i>
                                </div>
                                <div class="dropdown-menu dropdown-menu-right custom-dropdown">
                                    <ul>
                                        <li>
                                            <a href=""><i class="icon-font-light iw-16 ih-16"
                                                    data-feather="bookmark"></i>save post</a>
                                        </li>
                                        <li>
                                            <a href=""><i class="icon-font-light iw-16 ih-16"
                                                    data-feather="x-square"></i>hide post</a>
                                        </li>
                                        <li>
                                            <a href=""><i class="icon-font-light iw-16 ih-16"
                                                    data-feather="x-octagon"></i>unfollow sufiya</a>
                                        </li>
                                    </ul>
                                </div>
                            </div>
                        </div>
                    </div>
                    <div class="post-details">
                        <div class="img-wrapper">
                            <img src="images/post/1.jpg" class="img-fluid blur-up lazyload"
                                alt="">
                            <div class="controler">
                                <a href="#" class="play" data-bs-toggle="modal" data-bs-target="#videoPlayer">
                                    <i class="iw-50 ih-50" data-feather="play-circle"></i>
                                </a>
                                <div class="duration">
                                    <h6>06:20</h6>
                                </div>
                                <a href="#" class="volume">
                                    <i class="iw-14 ih-14" data-feather="volume-2"></i>
                                </a>
                            </div>
                        </div>
                        <div class="detail-box">
                            <h3>Today Our Three Cute Puppy Dog Birthday !!!!</h3>
                            <h5 class="tag"><span>#ourcutepuppy,</span> #puppy, #birthday, #dog</h5>
                            <p>Lorem Ipsum is simply dummy text of the printing and typesetting industry.
                                has been the industry's standard dummy text ever since the 1500s</p>
                            <div class="bookmark favourite-btn">
                                <i class="iw-14 ih-14" data-feather="bookmark"></i>
                            </div>
                            <div class="people-likes">
                                <ul>
                                    <li class="popover-cls" data-bs-toggle="popover" data-placement="right"
                                        data-name="sufiya eliza" data-img="images/user-sm/1.jpg">
                                        <img src="images/user-sm/1.jpg"
                                            class="img-fluid blur-up lazyload bg-img" alt="">
                                    </li>
                                    <li class="popover-cls" data-bs-toggle="popover" data-placement="right"
                                        data-name="sufiya eliza" data-img="images/user-sm/2.jpg">
                                        <img src="images/user-sm/2.jpg"
                                            class="img-fluid blur-up lazyload bg-img" alt="">
                                    </li>
                                    <li class="popover-cls" data-bs-toggle="popover" data-placement="right"
                                        data-name="sufiya eliza" data-img="images/user-sm/3.jpg">
                                        <img src="images/user-sm/3.jpg"
                                            class="img-fluid blur-up lazyload bg-img" alt="">
                                    </li>
                                </ul>
                                <h6>+12 people react this post</h6>
                            </div>
                        </div>
                        <div class="like-panel">
                            <div class="left-emoji">
                                <ul>
                                    <li>
                                        <img src="svg/emoji/040.svg" alt="smile">
                                    </li>
                                    <li>
                                        <img src="svg/emoji/113.svg" alt="heart">
                                    </li>
                                    <li>
                                        <img src="svg/emoji/027.svg" alt="cry">
                                    </li>
                                    <li>
                                        <img src="svg/emoji/033.svg" alt="angry">
                                    </li>
                                </ul>
                                <h6>+75</h6>
                            </div>
                            <div class="right-stats">
                                <ul>
                                    <li>
                                        <h5>
                                            <i class="iw-16 ih-16" data-feather="message-square"></i>
                                            <span>4565</span> comment
                                        </h5>
                                    </li>
                                    <li>
                                        <h5>
                                            <i class="iw-16 ih-16" data-feather="share"></i><span>985</span>
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
                                        <i class="iw-18 ih-18" data-feather="smile"></i> react
                                    </a>
                                    <div class="react-box">
                                        <ul>
                                            <li data-title="smile">
                                                <a href="javascript:void(0)">
                                                    <img src="svg/emoji/040.svg" alt="smile">
                                                </a>
                                            </li>
                                            <li data-title="love">
                                                <a href="javascript:void(0)">
                                                    <img src="svg/emoji/113.svg" alt="heart">
                                                </a>
                                            </li>
                                            <li data-title="cry">
                                                <a href="javascript:void(0)">
                                                    <img src="svg/emoji/027.svg" alt="cry">
                                                </a>
                                            </li>
                                            <li data-title="wow">
                                                <a href="javascript:void(0)">
                                                    <img src="svg/emoji/052.svg" alt="angry">
                                                </a>
                                            </li>
                                            <li data-title="angry">
                                                <a href="javascript:void(0)">
                                                    <img src="svg/emoji/039.svg" alt="angry">
                                                </a>
                                            </li>
                                            <li data-title="haha">
                                                <a href="javascript:void(0)">
                                                    <img src="svg/emoji/042.svg" alt="">
                                                </a>
                                            </li>
                                        </ul>
                                    </div>
                                </li>
                                <li class="comment-click">
                                    <a href="javascript:void(0)">
                                        <i class="iw-18 ih-18" data-feather="message-square"></i> comment
                                    </a>
                                </li>
                                <li data-bs-target="#shareModal" data-bs-toggle="modal">
                                    <a href="javascript:void(0)">
                                        <i class="iw-16 ih-16" data-feather="share"></i> share
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
                                        <a href="#" class="user-img popover-cls" data-bs-toggle="popover"
                                            data-placement="right" data-name="Pabelo mukrani"
                                            data-img="images/user-sm/2.jpg">
                                            <img src="images/user-sm/2.jpg"
                                                class="img-fluid blur-up lazyload bg-img" alt="user">
                                        </a>
                                        <div class="media-body">
                                            <a href="#">
                                                <h5>Pabelo Mukrani</h5>
                                            </a>
                                            <p>Oooo Very Cute and Sweet Dog, happy birthday Cuty....
                                                &#128578;
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
                                            <a href="#" class="user-img popover-cls" data-bs-toggle="popover"
                                                data-placement="right" data-name="sufiya elija"
                                                data-img="images/user-sm/3.jpg">
                                                <img src="images/user-sm/3.jpg"
                                                    class="img-fluid blur-up lazyload bg-img" alt="user">
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
                                            <a href="#" class="user-img popover-cls" data-bs-toggle="popover"
                                                data-placement="right" data-name="sufiya eliza"
                                                data-img="images/user-sm/4.jpg">
                                                <img src="images/user-sm/4.jpg"
                                                    class="img-fluid blur-up lazyload bg-img" alt="user">
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
                                        <a href="javascript:void(0)" class="load">
                                            <i class="iw-15 ih-15 fas fa-rotate"></i> load more
                                            replies
                                        </a>
                                    </div>
                                </div>
                                <div class="main-comment">
                                    <div class="media">
                                        <a href="#" class="user-img popover-cls" data-bs-toggle="popover"
                                            data-placement="right" data-name="pabelo mukrani"
                                            data-img="images/user-sm/2.jpg">
                                            <img src="images/user-sm/2.jpg"
                                                class="img-fluid blur-up lazyload bg-img" alt="user">
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
                                    <input type="text" class="form-control emojiPicker"
                                        placeholder="write a comment..">
                                    <a href="javascript:void(0)">
                                        <i data-feather="smile" class="icon icon-2 iw-14 ih-14"></i>
                                    </a>
                                    <a href="javascript:void(0)">
                                        <i class="iw-14 ih-14 icon" data-feather="camera"></i>
                                    </a>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
            <div id="load-more" class="post-loader">
                <div class="loader-icon">
                    <i class="icon-theme iw-25 ih-25" data-feather="rotate-ccw"></i>
                </div>
                <div class="no-more-text">
                    <p>no more post</p>
                </div>
            </div>
        </div>
        <div class="content-right">
            <!-- birthday reminder -->
            <div class="birthday-section bg-size blur-up lazyloaded" style="background-image: url(&quot;images/birthday-bg.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                <img src="images/birthday-bg.jpg" class="img-fluid blur-up lazyload bg-img" alt="birthday" style="display: none;">
                <div class="birthday-top">
                    <div class="title">
                        <h3>birthday !!!!</h3>
                        <h6>today your collge friend's birthday</h6>
                    </div>
                    <div class="setting">
                        <div class="setting-btn light-btn">
                            <a href=/# class="d-flex">
                                <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-rotate-cw icon icon-light stroke-width-3 iw-11 ih-11"><polyline points="23 4 23 10 17 10"></polyline><path d="M20.49 15a9 9 0 1 1-2.12-9.36L23 10"></path></svg>
                            </a>
                        </div>
                        <div class="setting-btn light-btn ms-2 setting-dropdown">
                            <div class="btn-group custom-dropdown arrow-none dropdown-sm">
                                <a class="d-flex" href=/# data-bs-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
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
                        <div class="icon">
                            <img src="images/icon/cake.png" class="img-fluid blur-up lazyloaded" alt="cake">
                        </div>
                        <div class="center-profile bg-size blur-up lazyloaded" style="background-image: url(&quot;images/user-sm/4.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                            <img src="images/user-sm/4.jpg" class="img-fluid blur-up lazyload bg-img" alt="user" style="display: none;">
                        </div>
                        <div class="icon">
                            <h5>20+</h5>
                        </div>
                    </div>
                    <div class="details">
                        <h3>sufiya elija</h3>
                        <h6>glasgow, scotland</h6>
                        <p>Lorem 5th Sept 2019 dummy text of the printing and typesetting industry.</p>
                        <form>
                            <input type="text" placeholder="wish birthday to your friend" class="form-control">
                            <button type="submit">
                                <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-arrow-right icon-light icon stroke-width-3 iw-13 ih-13"><line x1="5" y1="12" x2="19" y2="12"></line><polyline points="12 5 19 12 12 19"></polyline></svg>
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
                                <a href=/#>
                                    <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-rotate-cw icon icon-dark stroke-width-3 iw-11 ih-11"><polyline points="23 4 23 10 17 10"></polyline><path d="M20.49 15a9 9 0 1 1-2.12-9.36L23 10"></path></svg>
                                </a>
                            </div>
                            <div class="setting-btn ms-2 setting-dropdown">
                                <div class="btn-group custom-dropdown arrow-none dropdown-sm">
                                    <a href=/# data-bs-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
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
                                        <a href="javascript:void(0)" data-bs-toggle="modal" data-bs-target="#imageModel" class="bg-size blur-up lazyloaded" style="background-image: url(&quot;images/story/1.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                                            <img src="images/story/1.jpg" alt="" class="img-fluid blur-up lazyload bg-img" style="display: none;">
                                        </a>
                                    </div>
                                </div>
                            </div>
                            <div class="col-4">
                                <div class="overlay">
                                    <div class="portfolio-image">
                                        <a href="javascript:void(0)" data-bs-toggle="modal" data-bs-target="#imageModel" class="bg-size blur-up lazyloaded" style="background-image: url(&quot;images/story/2.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                                            <img src="images/story/2.jpg" alt="" class="img-fluid blur-up lazyload bg-img" style="display: none;">
                                        </a>
                                    </div>
                                </div>
                            </div>
                            <div class="col-4">
                                <div class="overlay">
                                    <div class="portfolio-image">
                                        <a href="javascript:void(0)" data-bs-toggle="modal" data-bs-target="#imageModel" class="bg-size blur-up lazyloaded" style="background-image: url(&quot;images/story/3.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                                            <img src="images/story/3.jpg" alt="" class="img-fluid blur-up lazyload bg-img" style="display: none;">
                                        </a>
                                    </div>
                                </div>
                            </div>
                            <div class="col-4 row m-0">
                                <div class="col-12 pt-cls p-0">
                                    <div class="overlay">
                                        <div class="portfolio-image">
                                            <a href="javascript:void(0)" data-bs-toggle="modal" data-bs-target="#imageModel" class="bg-size blur-up lazyloaded" style="background-image: url(&quot;images/story/4.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                                                <img src="images/story/4.jpg" alt="" class="img-fluid blur-up lazyload bg-img" style="display: none;">
                                            </a>
                                        </div>
                                    </div>
                                </div>
                                <div class="col-12 pt-cls p-0">
                                    <div class="overlay">
                                        <div class="portfolio-image">
                                            <a href="javascript:void(0)" data-bs-toggle="modal" data-bs-target="#imageModel" class="bg-size blur-up lazyloaded" style="background-image: url(&quot;images/story/6.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                                                <img src="images/story/6.jpg" alt="" class="img-fluid blur-up lazyload bg-img" style="display: none;">
                                            </a>
                                        </div>
                                    </div>
                                </div>
                            </div>
                            <div class="col-8 pt-cls">
                                <div class="overlay">
                                    <div class="portfolio-image">
                                        <a href="javascript:void(0)" data-bs-toggle="modal" data-bs-target="#imageModel" class="bg-size blur-up lazyloaded" style="background-image: url(&quot;images/story/5.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                                            <img src="images/story/5.jpg" alt="" class="img-fluid blur-up lazyload bg-img" style="display: none;">
                                        </a>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
            <div class="sticky-top">
                <!-- event -->
                <div class="event-box section-t-space ratio2_3">
                    <div class="image-section bg-size blur-up lazyloaded" style="background-image: url(&quot;images/event/1.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                        <img src="images/event/1.jpg" class="img-fluid blur-up lazyload bg-img" alt="event" style="display: none;">
                        <div class="card-title">
                            <h3>event</h3>
                            <div class="settings">
                                <div class="setting-btn">
                                    <a href=/# class="d-flex">
                                        <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-rotate-cw icon icon-dark stroke-width-3 iw-11 ih-11"><polyline points="23 4 23 10 17 10"></polyline><path d="M20.49 15a9 9 0 1 1-2.12-9.36L23 10"></path></svg>
                                    </a>
                                </div>
                                <div class="setting-btn ms-2 setting-dropdown">
                                    <div class="btn-group custom-dropdown arrow-none dropdown-sm">
                                        <a href=/# data-bs-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
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
                            <img src="images/icon/play.png" class="img-fluid blur-up lazyloaded" alt="play">
                        </div>
                    </div>
                    <div class="event-content">
                        <h3>christmas 2021</h3>
                        <h6>26 january 2021</h6>
                        <p>Lorem Ipsum is simply dummy text of the printing and typesetting industry
                            <span>15256 People Going</span></p>
                        <div class="bottom-part">
                            <a href=/# class="event-btn">going / not going</a>
                        </div>
                        <a href=/# class="share-btn">
                            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-corner-up-right icon-dark stroke-width-3 iw-14 ih-14"><polyline points="15 14 20 9 15 4"></polyline><path d="M4 20v-7a4 4 0 0 1 4-4h12"></path></svg>
                        </a>
                    </div>
                </div>

                <!-- suggestion box -->
                <div class="suggestion-box section-t-space">
                    <div class="card-title">
                        <h3>your games</h3>
                        <h5>24 games</h5>
                        <div class="settings">
                            <div class="setting-btn">
                                <a href=/# class="d-flex">
                                    <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-rotate-cw icon icon-dark stroke-width-3 iw-11 ih-11"><polyline points="23 4 23 10 17 10"></polyline><path d="M20.49 15a9 9 0 1 1-2.12-9.36L23 10"></path></svg>
                                </a>
                            </div>
                            <div class="setting-btn setting-dropdown ms-2">
                                <div class="btn-group custom-dropdown arrow-none dropdown-sm">
                                    <a href=/# data-bs-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
                                        <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-sun icon-dark stroke-width-3 icon iw-11 ih-11"><circle cx="12" cy="12" r="5"></circle><line x1="12" y1="1" x2="12" y2="3"></line><line x1="12" y1="21" x2="12" y2="23"></line><line x1="4.22" y1="4.22" x2="5.64" y2="5.64"></line><line x1="18.36" y1="18.36" x2="19.78" y2="19.78"></line><line x1="1" y1="12" x2="3" y2="12"></line><line x1="21" y1="12" x2="23" y2="12"></line><line x1="4.22" y1="19.78" x2="5.64" y2="18.36"></line><line x1="18.36" y1="5.64" x2="19.78" y2="4.22"></line></svg>
                                    </a>
                                    <div class="dropdown-menu dropdown-menu-right custom-dropdown">
                                        <ul>
                                            <li>
                                                <a href=""><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-user icon-font-light iw-16 ih-16"><path d="M20 21v-2a4 4 0 0 0-4-4H8a4 4 0 0 0-4 4v2"></path><circle cx="12" cy="7" r="4"></circle></svg>see all</a>
                                            </li>
                                            <li>
                                                <a href=""><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-search icon-font-light iw-16 ih-16"><circle cx="11" cy="11" r="8"></circle><line x1="21" y1="21" x2="16.65" y2="16.65"></line></svg>find
                                                    friends</a>
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
                        <div class="slide-2 no-arrow default-space slick-initialized slick-slider"><button class="slick-prev slick-arrow" aria-label="Previous" type="button" aria-disabled="false" style="display: inline-block;">Previous</button><div class="slick-list draggable"><div class="slick-track" style="opacity: 1; width: 405px; transform: translate3d(-135px, 0px, 0px);"><div class="slick-slide" data-slick-index="0" aria-hidden="true" style="width: 135px;" tabindex="-1"><div><div style="width: 100%; display: inline-block;">
                                <div class="story-box">
                                    <div class="adaptive-overlay"></div>
                                    <div class="story-bg bg-size" style="background-image: url(&quot;images/game/1.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                                        <img src="images/game/1.jpg" class="img-fluid bg-img" data-adaptive-background="1" alt="" style="display: none;">
                                    </div>
                                    <div class="story-content">
                                        <h6>josephin water</h6>
                                        <span class="player"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-user icon-light iw-10 ih-10"><path d="M20 21v-2a4 4 0 0 0-4-4H8a4 4 0 0 0-4 4v2"></path><circle cx="12" cy="7" r="4"></circle></svg>15k</span>
                                    </div>
                                </div>
                            </div></div></div><div class="slick-slide slick-current slick-active" data-slick-index="1" aria-hidden="false" style="width: 135px;"><div><div style="width: 100%; display: inline-block;">
                                <div class="story-box">
                                    <div class="adaptive-overlay"></div>
                                    <div class="story-bg bg-size" style="background-image: url(&quot;images/game/2.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                                        <img src="images/game/2.jpg" class="img-fluid bg-img" data-adaptive-background="1" alt="" style="display: none;">
                                    </div>
                                    <div class="story-content">
                                        <h6>josephin water</h6>
                                        <span class="player"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-user icon-light iw-10 ih-10"><path d="M20 21v-2a4 4 0 0 0-4-4H8a4 4 0 0 0-4 4v2"></path><circle cx="12" cy="7" r="4"></circle></svg>30k</span>
                                    </div>
                                </div>
                            </div></div></div><div class="slick-slide slick-active" data-slick-index="2" aria-hidden="false" style="width: 135px;"><div><div style="width: 100%; display: inline-block;">
                                <div class="story-box">
                                    <div class="adaptive-overlay"></div>
                                    <div class="story-bg bg-size" style="background-image: url(&quot;images/game/3.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                                        <img src="images/game/3.jpg" class="img-fluid bg-img" data-adaptive-background="1" alt="" style="display: none;">
                                    </div>
                                    <div class="story-content">
                                        <h6>josephin water</h6>
                                        <span class="player"> <img src="images/icon/user-w.png" class="img-fluid blur-up lazyload" alt="">25k</span>
                                    </div>
                                </div>
                            </div></div></div></div></div><button class="slick-next slick-arrow slick-disabled" aria-label="Next" type="button" style="display: inline-block;" aria-disabled="true">Next</button></div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</div>