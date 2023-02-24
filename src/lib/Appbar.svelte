<script>
    import AppBox from "./appBox.svelte";

    let recentSearch;
    let appbox = false;
    let toggleAppBox = () => appbox = !appbox;
</script>
<!-- header -->
<header>
    <div class="mobile-fix-menu d-md-none inline-flex">
        <ul class="flex text-slate-50 items-center justify-evenly w-full relative">
            <li class="border-x-white border-r flex-grow h-full">
                <a href="index.html" title="Home" data-toggle="tooltip">
                    <i>
                        <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" viewBox="0 0 24 24"
                            fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" 
                            class="feather feather-home">
                            <path d="M3 9l9-7 9 7v11a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2z"/>
                            <polyline points="9 22 9 12 15 12 15 22" />
                        </svg>
                    </i>
                </a>
            </li>
            <li class="border-x-white border-r flex-grow h-full relative">
                <a
                    class="mesg-notif"
                    href="index.html#"
                    title="Messages"
                    data-toggle="tooltip"
                >
                    <i>
                        <svg
                            xmlns="http://www.w3.org/2000/svg"
                            width="16"
                            height="16"
                            viewBox="0 0 24 24"
                            fill="none"
                            stroke="currentColor"
                            stroke-width="2"
                            stroke-linecap="round"
                            stroke-linejoin="round"
                            class="feather feather-message-square"
                        >
                            <path
                                d="M21 15a2 2 0 0 1-2 2H7l-4 4V5a2 2 0 0 1 2-2h14a2 2 0 0 1 2 2z"
                            />
                        </svg></i
                    >
                </a>
                <span class="notify-badge" />
            </li>
            <li class="border-x-white border-r flex-grow h-full relative">
                <a class="mesg-notif" href="index.html#" title="Notifications" data-toggle="tooltip">
                    <i>
                        <svg
                            xmlns="http://www.w3.org/2000/svg"
                            width="16"
                            height="16"
                            viewBox="0 0 24 24"
                            fill="none"
                            stroke="currentColor"
                            stroke-width="2"
                            stroke-linecap="round"
                            stroke-linejoin="round"
                            class="feather feather-bell">
                            <path
                                d="M18 8A6 6 0 0 0 6 8c0 7-3 9-3 9h18s-3-2-3-9"
                            />
                            <path d="M13.73 21a2 2 0 0 1-3.46 0" />
                        </svg></i
                    >
                </a>
                <span class="notify-badge" />
            </li>
            <li class="border-x-white border-r flex-grow h-full relative">
                <a class="mesg-notif" href="index.html#" title="Friend Request" data-toggle="tooltip">
                    <i class="">
                        <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-user-plus icon-light stroke-width-3 iw-16 ih-16"><path d="M16 21v-2a4 4 0 0 0-4-4H5a4 4 0 0 0-4 4v2"></path><circle cx="8.5" cy="7" r="4"></circle><line x1="20" y1="8" x2="20" y2="14"></line><line x1="23" y1="11" x2="17" y2="11"></line></svg>
                    </i>  
                </a>
                <span class="notify-badge" />
            </li>
            <li class="border-x-white border-r flex-grow h-full">
                <a class="create" href="index.html#" title="Add New" data-toggle="tooltip">
                    <i>
                        <svg
                            xmlns="http://www.w3.org/2000/svg"
                            width="16"
                            height="16"
                            viewBox="0 0 24 24"
                            fill="none"
                            stroke="currentColor"
                            stroke-width="2"
                            stroke-linecap="round"
                            stroke-linejoin="round"
                            class="feather feather-plus">
                            <line x1="12" y1="5" x2="12" y2="19" />
                            <line x1="5" y1="12" x2="19" y2="12" />
                        </svg>
                    </i>
                </a>
            </li>
            <li class="flex-grow">
                <a href="#" title="" on:click|preventDefault={()=> toggleAppBox()}>
                    <i>
                        <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" viewBox="0 0 24 24" fill="none" 
                            stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" 
                            class="feather feather-grid" >
                            <rect x="3" y="3" width="7" height="7" />
                            <rect x="14" y="3" width="7" height="7" />
                            <rect x="14" y="14" width="7" height="7" />
                            <rect x="3" y="14" width="7" height="7" />
                        </svg>
                    </i>
                </a>
                {#if appbox}
                <AppBox />
                {/if}
            </li>
        </ul>
    </div>
    <div class="container-fluid custom-padding">
        <div class="header-section relative">
            <div class="header-left">
                <div class="brand-logo">
                    <a href="index.html">
                        <img
                            src="images/logo (2).png"
                            alt="logo"
                            class="img-fluid lazyload"
                        />
                    </a>
                </div>
                <div class="searches">
                    <form method="post">
                        <input type="text" placeholder="Search..." on:focusout={() => recentSearch.classList.remove("active")}
                            on:focusin={() => recentSearch.classList.add("active")}/>
                        <button type="submit" ><i class="text-white fas fa-search" /></button>
                        <span class="cancel-search"><i class="fas fa-times" /></span>
                        <div class="recent-search" bind:this={recentSearch}>
                            <h4 class="recent-searches">Your's Recent Search </h4>
                            <ul class="so-history">
                                <li>
                                    <div class="searched-user">
                                        <figure>
                                            <img src="images/resources/user1.jpg" alt=""/>
                                        </figure>
                                        <span>Danial Carabal</span>
                                    </div>
                                    <span class="trash"><i class="fas fa-times"/></span>
                                </li>
                                <li>
                                    <div class="searched-user">
                                        <figure>
                                            <img
                                                src="images/resources/user1.jpg"
                                                alt=""
                                            />
                                        </figure>
                                        <span>Danial Carabal</span>
                                    </div>
                                    <span class="trash" ><i class="fas fa-times"/></span>
                                </li>
                                <li>
                                    <div class="searched-user">
                                        <figure>
                                            <img
                                                src="images/resources/user1.jpg"
                                                alt=""
                                            />
                                        </figure>
                                        <span>Danial Carabal</span>
                                    </div>
                                    <span class="trash"
                                        ><i
                                            class="fas fa-times"
                                        /></span
                                    >
                                </li>
                                <li>
                                    <div class="searched-user">
                                        <figure>
                                            <img
                                                src="images/resources/user1.jpg"
                                                alt=""
                                            />
                                        </figure>
                                        <span>Danial Carabal</span>
                                    </div>
                                    <span class="trash"
                                        ><i
                                            class="fas fa-times"
                                        /></span
                                    >
                                </li>
                                <li>
                                    <div class="searched-user">
                                        <figure>
                                            <img
                                                src="images/resources/user1.jpg"
                                                alt=""
                                            />
                                        </figure>
                                        <span>Danial Carabal</span>
                                    </div>
                                    <span class="trash"
                                        ><i
                                            class="fas fa-times"
                                        /></span
                                    >
                                </li>
                                <li>
                                    <div class="searched-user">
                                        <figure>
                                            <img
                                                src="images/resources/user1.jpg"
                                                alt=""
                                            />
                                        </figure>
                                        <span>Danial Carabal</span>
                                    </div>
                                    <span class="trash"
                                        ><i
                                            class="fas fa-times"
                                        /></span
                                    >
                                </li>
                                <li>
                                    <div class="searched-user">
                                        <figure>
                                            <img
                                                src="images/resources/user1.jpg"
                                                alt=""
                                            />
                                        </figure>
                                        <span>Danial Carabal</span>
                                    </div>
                                    <span class="trash"
                                        ><i
                                            class="fas fa-times"
                                        /></span
                                    >
                                </li>
                                <li>
                                    <div class="searched-user">
                                        <figure>
                                            <img
                                                src="images/resources/user1.jpg"
                                                alt=""
                                            />
                                        </figure>
                                        <span>Danial Carabal</span>
                                    </div>
                                    <span class="trash"
                                        ><i
                                            class="fas fa-times"
                                        /></span
                                    >
                                </li>
                                <li>
                                    <div class="searched-user">
                                        <figure>
                                            <img
                                                src="images/resources/user1.jpg"
                                                alt=""
                                            />
                                        </figure>
                                        <span>Danial Carabal</span>
                                    </div>
                                    <span class="trash"
                                        ><i
                                            class="fas fa-times"
                                        /></span
                                    >
                                </li>
                                <li>
                                    <div class="searched-user">
                                        <figure>
                                            <img
                                                src="images/resources/user1.jpg"
                                                alt=""
                                            />
                                        </figure>
                                        <span>Danial Carabal</span>
                                    </div>
                                    <span class="trash"
                                        ><i
                                            class="fas fa-times"
                                        /></span
                                    >
                                </li>
                                <li>
                                    <div class="searched-user">
                                        <figure>
                                            <img
                                                src="images/resources/user1.jpg"
                                                alt=""
                                            />
                                        </figure>
                                        <span>Danial Carabal</span>
                                    </div>
                                    <span class="trash"
                                        ><i
                                            class="fas fa-times"
                                        /></span
                                    >
                                </li>
                                <li>
                                    <div class="searched-user">
                                        <figure>
                                            <img
                                                src="images/resources/user2.jpg"
                                                alt=""
                                            />
                                        </figure>
                                        <span>Maria K</span>
                                    </div>
                                    <span class="trash"
                                        ><i
                                            class="fas fa-times"
                                        /></span
                                    >
                                </li>
                                <li>
                                    <div class="searched-user">
                                        <figure>
                                            <img
                                                src="images/resources/user3.jpg"
                                                alt=""
                                            />
                                        </figure>
                                        <span>Fawad Khan</span>
                                    </div>
                                    <span class="trash"
                                        ><i
                                            class="fas fa-times"
                                        /></span
                                    >
                                </li>
                                <li>
                                    <div class="searched-user">
                                        <figure>
                                            <img
                                                src="images/resources/user4.jpg"
                                                alt=""
                                            />
                                        </figure>
                                        <span>Danial Sandos</span>
                                    </div>
                                    <span class="trash"
                                        ><i
                                            class="fas fa-times"
                                        /></span
                                    >
                                </li>
                                <li>
                                    <div class="searched-user">
                                        <figure>
                                            <img
                                                src="images/resources/user5.jpg"
                                                alt=""
                                            />
                                        </figure>
                                        <span>Jack Carter</span>
                                    </div>
                                    <span class="trash"
                                        ><i
                                            class="fas fa-times"
                                        /></span
                                    >
                                </li>
                            </ul>
                        </div>
                    </form>
                </div>
            </div>
            <div class="header-right relative flex">
                <ul class="web-elements flex items-center relative justify-around">
                    <li class="z-0">
                        <div class="user-dp lg:p-1 lg:pr-2.5">
                            <a href="profile-page2.html" title="" class="flex items-center">
                                <img alt="" src="images/resources/user.jpg" />
                                <div class="name hidden p-1 sm:inline-block md:hidden lg:inline-block">
                                    <h4 class="text-ellipsis whitespace-nowrap">Danial Cardos</h4>
                                </div>
                            </a>
                        </div>
                    </li>
                    <div class="flex">
                        <li class="go-live hidden sm:inline-block z-0">
                            <a
                            href="live-stream.html"
                            title="Go Live"
                            data-toggle="tooltip"
                            >
                            <i>
                                <svg
                                fill="#f00"
                                    xmlns="http://www.w3.org/2000/svg"
                                    viewBox="0 0 32 32"
                                    width="18px"
                                    height="18px"
                                >
                                <path
                                        d="M 6.1015625 6.1015625 C 3.5675625 8.6345625 2 12.134 2 16 C 2 19.866 3.5675625 23.365437 6.1015625 25.898438 L 7.5195312 24.480469 C 5.3465312 22.307469 4 19.308 4 16 C 4 12.692 5.3465312 9.6925313 7.5195312 7.5195312 L 6.1015625 6.1015625 z M 25.898438 6.1015625 L 24.480469 7.5195312 C 26.653469 9.6925312 28 12.692 28 16 C 28 19.308 26.653469 22.307469 24.480469 24.480469 L 25.898438 25.898438 C 28.432437 23.365437 30 19.866 30 16 C 30 12.134 28.432437 8.6345625 25.898438 6.1015625 z M 9.6367188 9.6367188 C 8.0077188 11.265719 7 13.515 7 16 C 7 18.485 8.0077187 20.734281 9.6367188 22.363281 L 11.052734 20.947266 C 9.7847344 19.680266 9 17.93 9 16 C 9 14.07 9.7847344 12.319734 11.052734 11.052734 L 9.6367188 9.6367188 z M 22.363281 9.6367188 L 20.947266 11.052734 C 22.215266 12.319734 23 14.07 23 16 C 23 17.93 22.215266 19.680266 20.947266 20.947266 L 22.363281 22.363281 C 23.992281 20.734281 25 18.485 25 16 C 25 13.515 23.992281 11.265719 22.363281 9.6367188 z M 16 12 A 4 4 0 0 0 16 20 A 4 4 0 0 0 16 12 z"
                                    />
                                </svg></i>
                            </a>
                        </li>
                        <li class="hidden md:inline-block">
                            <a href="index.html" title="Home" data-toggle="tooltip">
                                <i>
                                    <svg
                                    xmlns="http://www.w3.org/2000/svg"
                                        width="16"
                                        height="16"
                                        viewBox="0 0 24 24"
                                        fill="none"
                                        stroke="currentColor"
                                        stroke-width="2"
                                        stroke-linecap="round"
                                        stroke-linejoin="round"
                                        class="feather feather-home"
                                    >
                                        <path
                                            d="M3 9l9-7 9 7v11a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2z"
                                        />
                                        <polyline points="9 22 9 12 15 12 15 22" />
                                    </svg></i
                                >
                            </a>
                        </li>
                        <li class="hidden md:inline-block">
                            <a class="mesg-notif" href="index.html#" title="Friend Request" data-toggle="tooltip">
                                <i class="">
                                    <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" 
                                    viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" 
                                    stroke-linecap="round" stroke-linejoin="round" class="feather 
                                    feather-user-plus stroke-width-3 iw-16 ih-16">
                                    <path d="M16 21v-2a4 4 0 0 0-4-4H5a4 4 0 0 0-4 4v2"></path>
                                    <circle cx="8.5" cy="7" r="4">
                                    </circle><line x1="20" y1="8" x2="20" y2="14"></line>
                                    <line x1="23" y1="11" x2="17" y2="11"></line></svg>
                                </i>
                            </a>
                        </li>
                        <li class="hidden md:inline-block">
                            <a
                                class="mesg-notif"
                                href="index.html#"
                                title="Messages"
                                data-toggle="tooltip"
                            >
                            <i>
                                <svg
                                        xmlns="http://www.w3.org/2000/svg"
                                        width="16"
                                        height="16"
                                        viewBox="0 0 24 24"
                                        fill="none"
                                        stroke="currentColor"
                                        stroke-width="2"
                                        stroke-linecap="round"
                                        stroke-linejoin="round"
                                        class="feather feather-message-square"
                                    >
                                        <path
                                            d="M21 15a2 2 0 0 1-2 2H7l-4 4V5a2 2 0 0 1 2-2h14a2 2 0 0 1 2 2z"
                                        />
                                    </svg></i
                                >
                            </a>
                            <span />
                        </li>
                        <li class="hidden md:inline-block">
                            <a
                                class="mesg-notif"
                                href="index.html#"
                                title="Notifications"
                                data-toggle="tooltip"
                            >
                            <i>
                                <svg
                                xmlns="http://www.w3.org/2000/svg"
                                width="16"
                                height="16"
                                viewBox="0 0 24 24"
                                fill="none"
                                stroke="currentColor"
                                stroke-width="2"
                                        stroke-linecap="round"
                                        stroke-linejoin="round"
                                        class="feather feather-bell"
                                    >
                                        <path
                                            d="M18 8A6 6 0 0 0 6 8c0 7-3 9-3 9h18s-3-2-3-9"
                                        />
                                        <path d="M13.73 21a2 2 0 0 1-3.46 0" />
                                    </svg></i
                                >
                            </a>
                            <span />
                        </li>
                        <li  class="z-0">
                            <a
                                class="create"
                                href="index.html#"
                                title="Add New"
                                data-toggle="tooltip"
                            >
                                <i>
                                    <svg
                                        xmlns="http://www.w3.org/2000/svg"
                                        width="16"
                                        height="16"
                                        viewBox="0 0 24 24"
                                        fill="none"
                                        stroke="currentColor"
                                        stroke-width="2"
                                        stroke-linecap="round"
                                        stroke-linejoin="round"
                                        class="feather feather-plus"
                                    >
                                        <line x1="12" y1="5" x2="12" y2="19" />
                                        <line x1="5" y1="12" x2="19" y2="12" />
                                    </svg></i
                                >
                            </a>
                        </li>
                        <li class="hidden md:inline-block">
                            <a href="index.html#" title="">
                                <i>
                                    <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" viewBox="0 0 24 24" fill="none" 
                                        stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" 
                                        class="feather feather-grid" >
                                        <rect x="3" y="3" width="7" height="7" />
                                        <rect x="14" y="3" width="7" height="7" />
                                        <rect x="14" y="14" width="7" height="7" />
                                        <rect x="3" y="14" width="7" height="7" />
                                    </svg>
                                </i>
                            </a>
                            <ul class="dropdown">
                                <li>
                                    <a href="profile.html" title=""
                                    ><i class="fas fa-user" /> Your Profile</a
                                    >
                                </li>
                                <li>
                                    <a href="add-new-course.html" title=""
                                    ><i class="fas fa-plus" /> New Course</a
                                    >
                                </li>
                                <li>
                                    <a
                                        class="invite-new"
                                        href="index.html#"
                                        title=""
                                        ><i class="icofont-brand-slideshare" /> Invite
                                        Collegue</a
                                    >
                                </li>
                                <li>
                                    <a href="pay-out.html" title=""
                                        ><i class="icofont-price" /> Payout</a
                                    >
                                </li>
                                <li>
                                    <a href="price-plan.html" title=""
                                        ><i class="icofont-flash" /> Upgrade</a
                                    >
                                </li>
                                <li>
                                    <a href="help-faq.html" title=""
                                    ><i class="icofont-question-circle" /> Help</a
                                    >
                                </li>
                                <li>
                                    <a href="settings.html" title=""
                                        ><i class="icofont-gear" /> Setting</a
                                    >
                                </li>
                                <li>
                                    <a href="privacy-n-policy.html" title=""
                                        ><i class="icofont-notepad" /> Privacy</a
                                        >
                                    </li>
                                <li>
                                    <a class="dark-mod" href="index.html#" title=""
                                        ><i class="icofont-moon" /> Dark Mode</a
                                    >
                                </li>
                                <li class="logout">
                                    <a href="sign-in.html" title=""
                                        ><i class="icofont-power" /> Logout</a
                                        >
                                    </li>
                            </ul>
                        </li>
                    </div>
                </ul>
            </div>
        </div>
    </div>
</header>