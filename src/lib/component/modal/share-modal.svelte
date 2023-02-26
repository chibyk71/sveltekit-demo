<script>
    import Modal from "./modal.svelte";
    export let show = false;
</script>
<Modal {show}> 
    <svelte:fragment slot="header">
        <div class="setting-dropdown">
            <div class=" btn-group custom-dropdown arrow-none dropdown-sm">
                <h5 data-bs-toggle="dropdown" aria-haspopup="true" aria-expanded="false">share as post <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-chevron-down iw-14"><polyline points="6 9 12 15 18 9"></polyline></svg></h5>
                <div class="dropdown-menu custom-dropdown">
                    <ul>
                        <li>
                            <a href="">share as post</a>
                        </li>
                        <li>
                            <a href="">on friend's feed</a>
                        </li>
                        <li>
                            <a href="">in a group</a>
                        </li>
                        <li>
                            <a href="">share as message</a>
                        </li>
                    </ul>
                </div>
            </div>
        </div>
        <button type="button" class="btn-close fa-solid fa-times" on:click={() => show = false} aria-label="Close">
            
        </button>
    </svelte:fragment>

    <svelte:fragment slot="body">
        <div class="user-info">
            <div class="media">
                <a href="#" class="user-img bg-size blur-up lazyloaded" style="background-image: url(&quot;images/user-sm/2.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                    <img src="images/user-sm/2.jpg" class="img-fluid blur-up lazyload bg-img" alt="user" style="display: none;">
                </a>
                <div class="media-body">
                    <a href="#">
                        <h5>Pabelo Mukrani</h5>
                    </a>
                    <div class="setting-dropdown">
                        <div class=" btn-group custom-dropdown arrow-none dropdown-sm">
                            <h6 data-bs-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
                                <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" 
                                stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" 
                                class="feather feather-globe icon-font-light left-icon iw-12 ih-12"><circle cx="12" cy="12" r="10">
                                </circle><line x1="2" y1="12" x2="22" y2="12"></line><path d="M12 2a15.3 15.3 0 0 1 4 10 15.3 15.3 0 0 
                                1-4 10 15.3 15.3 0 0 1-4-10 15.3 15.3 0 0 1 4-10z"></path></svg>public 
                                <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" 
                                stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" 
                                class="feather feather-chevron-down iw-14"><polyline points="6 9 12 15 18 9"></polyline></svg>
                            </h6>
                            <div class="dropdown-menu custom-dropdown show">
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
                </div>
            </div>
        </div>
        <div class="input-section">
            <input type="text" class="form-control emojiPicker" placeholder="write a comment..">
        </div>
        <div class="post-section ratio2_1">
            <div class="post-img bg-size blur-up lazyloaded" style="background-image: url(&quot;images/post/1.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                <img src="images/post/1.jpg" class="img-fluid blur-up lazyload bg-img" alt="" style="display: none;">
            </div>
            <div class="post-content">
                <h3>Today Our Three Cute Puppy Dog Birthday !!!!</h3>
                <h5 class="tag"><span>#ourcutepuppy,</span> #puppy, #birthday, #dog</h5>
            </div>
        </div>
    </svelte:fragment>

    <svelte:fragment slot="footer">  
        <button type="button" class="btn btn-solid">share post</button>
    </svelte:fragment>
</Modal>
<!-- <div class="modal fade mobile-full-width show" id="shareModal" tabindex="-1" aria-labelledby="exampleModalLabel" aria-modal="true" role="dialog" style="display: block;">
    <div class="modal-dialog modal-dialog-centered" role="document">
        <div class="modal-content share-modal">
            <div class="modal-header">
                <div class="setting-dropdown">
                    <div class=" btn-group custom-dropdown arrow-none dropdown-sm">
                        <h5 data-bs-toggle="dropdown" aria-haspopup="true" aria-expanded="false">share as post <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-chevron-down iw-14"><polyline points="6 9 12 15 18 9"></polyline></svg></h5>
                        <div class="dropdown-menu custom-dropdown">
                            <ul>
                                <li>
                                    <a href="">share as post</a>
                                </li>
                                <li>
                                    <a href="">on friend's feed</a>
                                </li>
                                <li>
                                    <a href="">in a group</a>
                                </li>
                                <li>
                                    <a href="">share as message</a>
                                </li>
                            </ul>
                        </div>
                    </div>
                </div>
                <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close">
                    
                </button>
            </div>
            <div class="modal-body">
                <div class="user-info">
                    <div class="media">
                        <a href="#" class="user-img bg-size blur-up lazyloaded" style="background-image: url(&quot;images/user-sm/2.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                            <img src="images/user-sm/2.jpg" class="img-fluid blur-up lazyload bg-img" alt="user" style="display: none;">
                        </a>
                        <div class="media-body">
                            <a href="#">
                                <h5>Pabelo Mukrani</h5>
                            </a>
                            <div class="setting-dropdown">
                                <div class=" btn-group custom-dropdown arrow-none dropdown-sm">
                                    <h6 data-bs-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
                                        <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" 
                                        stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" 
                                        class="feather feather-globe icon-font-light left-icon iw-12 ih-12"><circle cx="12" cy="12" r="10">
                                        </circle><line x1="2" y1="12" x2="22" y2="12"></line><path d="M12 2a15.3 15.3 0 0 1 4 10 15.3 15.3 0 0 
                                        1-4 10 15.3 15.3 0 0 1-4-10 15.3 15.3 0 0 1 4-10z"></path></svg>public 
                                        <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" 
                                        stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" 
                                        class="feather feather-chevron-down iw-14"><polyline points="6 9 12 15 18 9"></polyline></svg>
                                    </h6>
                                    <div class="dropdown-menu custom-dropdown show">
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
                        </div>
                    </div>
                </div>
                <div class="input-section">
                    <input type="text" class="form-control emojiPicker" placeholder="write a comment..">
                </div>
                <div class="post-section ratio2_1">
                    <div class="post-img bg-size blur-up lazyloaded" style="background-image: url(&quot;images/post/1.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
                        <img src="images/post/1.jpg" class="img-fluid blur-up lazyload bg-img" alt="" style="display: none;">
                    </div>
                    <div class="post-content">
                        <h3>Today Our Three Cute Puppy Dog Birthday !!!!</h3>
                        <h5 class="tag"><span>#ourcutepuppy,</span> #puppy, #birthday, #dog</h5>
                    </div>
                </div>
            </div>
            <div class="modal-footer">
                <button type="button" class="btn btn-solid">share post</button>
            </div>
        </div>
    </div>
</div> -->