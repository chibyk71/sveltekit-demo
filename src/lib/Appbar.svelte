<script>
    import { Button } from "flowbite-svelte";
    import { tweened } from "svelte/motion";
    let value = "";

    $: icon = value?.trim() == "" && !value ? true : false;
    /**
     * @type {HTMLDivElement}
     */
    let recentSearch;
    let searchBock = 0;
    const swidth = tweened(searchBock);
    $: swidth.set(searchBock);
    $: sc = $swidth == 0 ? "hidden" : "";
    /**
     * @param {MouseEvent} e
     */
    function toggleDarkMode(e) {
        throw new Error("Function not implemented.");
    }
</script>

<div class="fixed container bg-blue-500 w-full md:hiden">
    <div
        style="width:{$swidth}%;"
        class="{sc} absolute left-0 top-0 bg-blue-500 w-full h-14 z-10 px-1 pt-1 overflow-hidden"
    >
        <form class="flex gap-px justify-center items-center w-full">
            {#if icon}
                <!-- content here -->
                <button
                    on:click={() => (searchBock = 100)}
                    class="uk-button uk-button-default"
                    ><i class="fas fa-times" /></button
                >
            {:else}
                <!-- else content here -->
                <button type="submit" class="uk-button uk-button-default"
                    ><i class="fas fa-search" /></button
                >`
            {/if}
            <!-- <Button pill={true} class="w-1/12  bg-transparent text-white" size="md"><span class="fas {icon}"></span></Button>   -->
            <input
                class="inline-block w-full"
                type="search"
                bind:value
                placeholder=""
                aria-label=""
            />
        </form>
    </div>
    <div
        class="flex gap-2 max-h-28 justify-between items-center py-1 min-w-full px-2 md:hidden"
    >
        <div class="logo res w-5/12">
            <img src="images/logo.png" alt="logo" />
            <span>Socimo</span>
        </div>
        <div class="user-avatar mobile w-4/12 self-center">
            <a href="profile.html" title="View Profile"
                ><img alt="" src="images/resources/user.jpg" /></a
            >
        </div>
        <Button
            pill={true}
            outline={true}
            on:click={() => (searchBock = 100)}
            class="w-1/12 bg-transparent text-white"
            size="md"><i class="fas fa-search" /></Button
        >
        <Button
            pill={true}
            outline={true}
            on:click={toggleDarkMode}
            class="w-1/12  bg-transparent text-white"
            size="md"><span class="fas fa-moon font-normal" /></Button
        >
    </div>
</div>

<header class="hidden md:flex">
    <div class="topbar stick">
        <div class="logo">
            <img src="images/logo.png" alt="" /><span>Socimo</span>
        </div>
        <div class="searches">
            <form method="post">
                <input
                    type="text"
                    placeholder="Search..."
                    on:focusout={() => recentSearch.classList.remove("active")}
                    on:focusin={() => recentSearch.classList.add("active")}
                />
                <button type="submit"><i class="icofont-search" /></button>
                <span class="cancel-search"><i class="icofont-close" /></span>
                <div class="recent-search" bind:this={recentSearch}>
                    <h4 class="recent-searches">Your's Recent Search</h4>
                    <ul class="so-history">
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
                                ><i class="icofont-close-circled" /></span
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
                                ><i class="icofont-close-circled" /></span
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
                                ><i class="icofont-close-circled" /></span
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
                                ><i class="icofont-close-circled" /></span
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
                                ><i class="icofont-close-circled" /></span
                            >
                        </li>
                    </ul>
                </div>
            </form>
        </div>

        <ul class="web-elements">
            <li>
                <div class="user-dp">
                    <a
                        href="profile-page2.html"
                        title=""
                        class="flex items-center"
                    >
                        <img alt="" src="images/resources/user.jpg" />
                        <div class="name">
                            <h4>Danial Cardos</h4>
                        </div>
                    </a>
                </div>
            </li>
            <li class="go-live">
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
                        </svg></i
                    >
                </a>
            </li>
            <li>
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
            <li>
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
            <li>
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
            <li>
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
            <li>
                <a href="index.html#" title="">
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
                            class="feather feather-grid"
                        >
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
                            ><i class="icofont-user-alt-3" /> Your Profile</a
                        >
                    </li>
                    <li>
                        <a href="add-new-course.html" title=""
                            ><i class="icofont-plus" /> New Course</a
                        >
                    </li>
                    <li>
                        <a class="invite-new" href="index.html#" title=""
                            ><i class="icofont-brand-slideshare" /> Invite Collegue</a
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
        </ul>
    </div>
</header>
<!-- header -->

<header>
    <div class="mobile-fix-menu" />
    <div class="container-fluid custom-padding">
        <div class="header-section">
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
                        <input
                            type="text"
                            placeholder="Search..."
                            on:focusout={() =>
                                recentSearch.classList.remove("active")}
                            on:focusin={() =>
                                recentSearch.classList.add("active")}
                        />
                        <button type="submit"
                            ><i class="text-white fas fa-search" /></button
                        >
                        <span class="cancel-search"
                            ><i class="text-white fas fa-times" /></span
                        >
                        <div class="recent-search" bind:this={recentSearch}>
                            <h4 class="recent-searches">
                                Your's Recent Search
                            </h4>
                            <ul class="so-history">
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
                                            class="icofont-close-circled"
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
                                            class="icofont-close-circled"
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
                                            class="icofont-close-circled"
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
                                            class="icofont-close-circled"
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
                                            class="icofont-close-circled"
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
                                            class="icofont-close-circled"
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
                                            class="icofont-close-circled"
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
                                            class="icofont-close-circled"
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
                                            class="icofont-close-circled"
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
                                            class="icofont-close-circled"
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
                                            class="icofont-close-circled"
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
                                            class="icofont-close-circled"
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
                                            class="icofont-close-circled"
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
                                            class="icofont-close-circled"
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
                                            class="icofont-close-circled"
                                        /></span
                                    >
                                </li>
                            </ul>
                        </div>
                    </form>
                </div>
                <ul class="btn-group">
                    <li class="header-btn home-btn">
                        <a class="main-link" href="index.html">
                            <i
                                class="icon-light stroke-width-3    h-4 fas fa-home"
                            />
                        </a>
                    </li>
                    <li
                        class="header-btn custom-dropdown dropdown-lg add-friend"
                    >
                        <a
                            class="main-link"
                            href="javascript:void(0)"
                            data-bs-toggle="dropdown"
                            aria-haspopup="true"
                            aria-expanded="false"
                        >
                            <i
                                class="icon-light stroke-width-3 w-4 h-4 fas fa-user-plus"
                            />
                        </a>
                        <div class="dropdown-menu">
                            <div class="dropdown-header">
                                <span>friend request</span>
                                <div class="mobile-close">
                                    <h5>close</h5>
                                </div>
                            </div>
                            <div class="dropdown-content">
                                <ul class="friend-list">
                                    <li>
                                        <div class="media">
                                            <img
                                                src="../assets/images/user-sm/5.jpg"
                                                alt="user"
                                            />
                                            <div class="media-body">
                                                <div>
                                                    <h5 class="mt-0">
                                                        Paige Turner
                                                    </h5>
                                                    <h6>1 mutual friend</h6>
                                                </div>
                                            </div>
                                        </div>
                                        <div class="action-btns">
                                            <button
                                                type="button"
                                                class="btn btn-solid"
                                                >confirm</button
                                            >
                                            <button
                                                type="button"
                                                class="btn btn-outline ms-1"
                                                >delete</button
                                            >
                                        </div>
                                    </li>
                                    <li>
                                        <div class="media">
                                            <img
                                                src="../assets/images/user-sm/6.jpg"
                                                alt="user"
                                            />
                                            <div class="media-body">
                                                <div>
                                                    <h5 class="mt-0">
                                                        Paige Turner
                                                    </h5>
                                                    <h6>1 mutual friend</h6>
                                                </div>
                                            </div>
                                        </div>
                                        <div class="action-btns">
                                            <button
                                                type="button"
                                                class="btn btn-solid"
                                                >confirm</button
                                            >
                                            <button
                                                type="button"
                                                class="btn btn-outline ms-1"
                                                >delete</button
                                            >
                                        </div>
                                    </li>
                                    <li>
                                        <div class="media">
                                            <img
                                                src="../assets/images/user-sm/7.jpg"
                                                alt="user"
                                            />
                                            <div class="media-body">
                                                <div>
                                                    <h5 class="mt-0">
                                                        Paige Turner
                                                    </h5>
                                                    <h6>1 mutual friend</h6>
                                                </div>
                                            </div>
                                        </div>
                                        <div class="action-btns">
                                            <button
                                                type="button"
                                                class="btn btn-solid"
                                                >confirm</button
                                            >
                                            <button
                                                type="button"
                                                class="btn btn-outline ms-1"
                                                >delete</button
                                            >
                                        </div>
                                    </li>
                                    <li>
                                        <div class="media">
                                            <img
                                                src="../assets/images/user-sm/2.jpg"
                                                alt="user"
                                            />
                                            <div class="media-body">
                                                <div>
                                                    <h5 class="mt-0">
                                                        Paige Turner
                                                    </h5>
                                                    <h6>1 mutual friend</h6>
                                                </div>
                                            </div>
                                        </div>
                                        <div class="action-btns">
                                            <button
                                                type="button"
                                                class="btn btn-solid"
                                                >confirm</button
                                            >
                                            <button
                                                type="button"
                                                class="btn btn-outline ms-1"
                                                >delete</button
                                            >
                                        </div>
                                    </li>
                                </ul>
                            </div>
                        </div>
                    </li>
                </ul>
            </div>
            <div class="header-right">
                <ul class="web-elements flex items-center">
                    <li>
                        <div class="user-dp">
                            <a href="profile-page2.html" title="" class="flex items-center">
                                <img alt="" src="images/resources/user.jpg" />
                                <div class="name">
                                    <h4>Danial Cardos</h4>
                                </div>
                            </a>
                        </div>
                    </li>
                    <li class="go-live">
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
                                </svg></i
                            >
                        </a>
                    </li>
                    <li>
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
                    <li>
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
                    <li>
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
                    <li>
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
                    <li>
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
                </ul>
            </div>
        </div>
    </div>
</header>
