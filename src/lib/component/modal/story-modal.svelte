<script>
	// your script goes here
	export let show = true
</script>

<style>
	/* your styles go here */
</style>

<!-- markup (zero or more items) goes here -->
{#if show}
<div class="modal story-model show fade" id="storyModel" tabindex="-1" role="dialog" aria-modal="true" style="display: block; padding-left: 0px;">
	<div class="modal-dialog modal-dialog-centered" role="document">
		<div class="modal-content">
			<div class="modal-body">
				<div class="story-bg">
					<div class="container-fluid p-0">
						<div class="row m-0">
							<div class="left-box col-xl-3 col-lg-4">
								<div class="model-title">
									<div class="title-main">
										<h2>stories</h2>
									</div>
									<div class="title-setting">
										<ul>
											<li><a href="#">archive</a></li>
											<li><a href="#">settings</a></li>
										</ul>
									</div>
								</div>
								<div class="modal-flex">
									<div class="add-story">
										<h4 class="story-title">your story</h4>
										<div class="media list-media">
											<div class="story-img" data-bs-toggle="modal" data-bs-target="#addStory">
												<div class="user-img bg-size blur-up lazyloaded" style="background-image: url(&quot;images/story-bg.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
													<img src="images/story-bg.jpg" class="img-fluid blur-up lazyload bg-img" alt="user" style="display: none;">
												</div>
												<div class="add-icon">
													<div class="icon">
														<img src="images/icon/plus.png" class="img-fluid blur-up lazyloaded" alt="plus">
													</div>
												</div>
											</div>
											<div class="media-body">
												<h5>add story</h5>
												<h6>share your photos or video</h6>
											</div>
										</div>
									</div>
									<div class="friend-story">
										<h4 class="story-title">all stories</h4>
										<div class="slider-nav slick-initialized slick-slider slick-vertical">
											<div class="slick-list draggable" style="height: 616px; padding: 50px 0px;">
												<div class="slick-track" style="opacity: 1; height: 462px; transform: translate3d(0px, 0px, 0px);">
													<div class="slick-slide" data-slick-index="0" aria-hidden="true" tabindex="-1" style="width: 270px;"><div><div style="width: 100%; display: inline-block;">
														<div class="media list-media">
															<div class="story-img seen">
																<div class="user-img bg-size blur-up lazyloaded" style="background-image: 
																	url(&quot;images/user-sm/1.jpg&quot;); background-size: cover; background-position: 
																		center center; background-repeat: no-repeat; display: block;">
																	<img src="images/user-sm/1.jpg" class="img-fluid blur-up lazyload bg-img" 
																	alt="user" style="display: none;">
																</div>
															</div>
															<div class="media-body">
																<h5>Petey Cruiser</h5>
																<h6>2 hours ago</h6>
															</div>
														</div>
													</div>
												</div>
											</div>
											<div class="slick-slide" data-slick-index="1" aria-hidden="true" tabindex="-1" style="width: 270px;"><div><div style="width: 100%; display: inline-block;">
												<div class="media list-media">
													<div class="story-img seen">
														<div class="user-img bg-size blur-up lazyloaded" style="background-image: url(&quot;images/user-sm/2.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
															<img src="images/user-sm/2.jpg" class="img-fluid blur-up lazyload bg-img" alt="user" style="display: none;">
														</div>
													</div>
													<div class="media-body">
														<h5>Anna Sthesia</h5>
														<h6>3 hours ago</h6>
													</div>
												</div>
											</div></div></div><div class="slick-slide" data-slick-index="2" aria-hidden="true" tabindex="-1" style="width: 270px;"><div><div style="width: 100%; display: inline-block;">
												<div class="media list-media">
													<div class="story-img">
														<div class="user-img bg-size blur-up lazyloaded" style="background-image: url(&quot;images/user-sm/3.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
															<img src="images/user-sm/3.jpg" class="img-fluid blur-up lazyload bg-img" alt="user" style="display: none;">
														</div>
													</div>
													<div class="media-body">
														<h5>Paul Molive</h5>
														<h6>5 hours ago</h6>
													</div>
												</div>
											</div></div></div><div class="slick-slide" data-slick-index="3" aria-hidden="true" tabindex="-1" style="width: 270px;"><div><div style="width: 100%; display: inline-block;">
												<div class="media list-media">
													<div class="story-img">
														<div class="user-img bg-size blur-up lazyloaded" style="background-image: url(&quot;images/user-sm/4.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
															<img src="images/user-sm/4.jpg" class="img-fluid blur-up lazyload bg-img" alt="user" style="display: none;">
														</div>
													</div>
													<div class="media-body">
														<h5>Anna Mull</h5>
														<h6>5 hours ago</h6>
													</div>
												</div>
											</div></div></div><div class="slick-slide" data-slick-index="4" aria-hidden="true" style="width: 270px;" tabindex="-1"><div><div style="width: 100%; display: inline-block;">
												<div class="media list-media">
													<div class="story-img">
														<div class="user-img bg-size blur-up lazyloaded" style="background-image: url(&quot;images/user-sm/5.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
															<img src="images/user-sm/5.jpg" class="img-fluid blur-up lazyload bg-img" alt="user" style="display: none;">
														</div>
													</div>
													<div class="media-body">
														<h5>Paige Turner</h5>
														<h6>5 hours ago</h6>
													</div>
												</div>
											</div></div></div><div class="slick-slide slick-current slick-center" data-slick-index="5" aria-hidden="true" style="width: 270px;"><div><div style="width: 100%; display: inline-block;">
												<div class="media list-media">
													<div class="story-img">
														<div class="user-img bg-size blur-up lazyloaded" style="background-image: url(&quot;images/user-sm/6.jpg&quot;); background-size: cover; background-position: center center; background-repeat: no-repeat; display: block;">
															<img src="images/user-sm/6.jpg" class="img-fluid blur-up lazyload bg-img" alt="user" style="display: none;">
														</div>
													</div>
													<div class="media-body">
														<h5>Bob Frapples</h5>
														<h6>5 hours ago</h6>
													</div>
												</div>
											</div></div></div></div></div></div>
									</div>
								</div>
							</div>
							<div class="right-box col-xl-9 col-lg-8 p-0">
								<a href="#" data-bs-dismiss="modal"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-x icon-light close"><line x1="18" y1="6" x2="6" y2="18"></line><line x1="6" y1="6" x2="18" y2="18"></line></svg></a>
								<div class="sliderContainer">
									<div class="slider single-item slick-initialized slick-slider">
										<div class="slick-list draggable">
											<div class="slick-track" style="opacity: 1; width: 5760px;">
												<div class="slick-slide" data-slick-index="0" aria-hidden="true" tabindex="-1" 
												style="width: 960px; position: relative; left: 0px; top: 0px; z-index: 998; opacity: 0; 
												transition: opacity 800ms ease 0s;"><div><div style="width: 100%; display: inline-block;">
													<div class="story-image"><img src="images/post/1.jpg" class="img-fluid blur-up lazyloaded" alt=""></div>
												</div>
											</div>
										</div>
										<div class="slick-slide" data-slick-index="1" aria-hidden="true" tabindex="-1" 
										style="width: 960px; position: relative; left: -960px; top: 0px; z-index: 998; opacity: 0; 
										transition: opacity 800ms ease 0s;">
											<div>
												<div style="width: 100%; display: inline-block;">
													<div class="story-image"><img src="images/post/2.jpg" class="img-fluid blur-up lazyloaded" alt=""></div>
												</div>
											</div>
										</div>
										<div class="slick-slide" data-slick-index="2" aria-hidden="true" tabindex="-1" style="width: 960px; 
											position: relative; left: -1920px; top: 0px; z-index: 998; opacity: 0; transition: opacity 800ms ease 
											0s;">
											<div>
												<div style="width: 100%; display: inline-block;">
													<div class="story-image"><img src="images/post/3.jpg" class="img-fluid blur-up lazyloaded" alt=""></div>
												</div>
											</div>
										</div>
										<div class="slick-slide" data-slick-index="3" aria-hidden="true" style="width: 960px; position: relative; left: -2880px; top: 0px; z-index: 998; opacity: 0; transition: opacity 800ms ease 0s;" tabindex="-1"><div><div style="width: 100%; display: inline-block;">
											<div class="story-image"><img src="images/post/4.jpg" class="img-fluid blur-up lazyloaded" alt=""></div>
												</div>
											</div>
										</div>
										<div class="slick-slide" data-slick-index="4" aria-hidden="true" style="width: 960px; position: relative; left: -3840px; top: 0px; z-index: 998; opacity: 0; transition: opacity 800ms ease 0s;" tabindex="-1"><div><div style="width: 100%; display: inline-block;">
											<div class="story-image"><img src="images/post/5.jpg" class="img-fluid blur-up lazyloaded" alt=""></div>
										</div></div></div><div class="slick-slide slick-current slick-active" data-slick-index="5" aria-hidden="false" style="width: 960px; position: relative; left: -4800px; top: 0px; z-index: 999; opacity: 1;"><div><div style="width: 100%; display: inline-block;">
											<div class="story-image"><img src="images/post/6.jpg" class="img-fluid blur-up lazyloaded" alt=""></div>
										</div></div></div></div></div></div>
									<div class="progressBarContainer">
										<div class="item">
											<span data-slick-index="0" class="progressBar"><div class="inProgress inProgress0" style="width: 100%;"></div></span>
										</div>
										<div class="item">
											<span data-slick-index="1" class="progressBar"><div class="inProgress inProgress1" style="width: 100%;"></div></span>
										</div>
										<div class="item">
											<span data-slick-index="2" class="progressBar"><div class="inProgress inProgress2" style="width: 100%;"></div></span>
										</div>
										<div class="item">
											<span data-slick-index="3" class="progressBar"><div class="inProgress inProgress3" style="width: 100%;"></div></span>
										</div>
										<div class="item">
											<span data-slick-index="4" class="progressBar"><div class="inProgress inProgress4" style="width: 100%;"></div></span>
										</div>
										<div class="item">
											<span data-slick-index="5" class="progressBar"><div class="inProgress inProgress5" style="width: 100%;"></div></span>
										</div>
									</div>
								</div>
								<div class="reply-section">
									<div class="reply-form">
										<input class="form-control" placeholder="reply...">
									</div>
									<ul class="emoji icon-xl">
										<li><img src="svg/emoji/040.svg" class="img-fluid blur-up lazyloaded" alt="smile">
										</li>
										<li><img src="svg/emoji/113.svg" class="img-fluid blur-up lazyloaded" alt="smile">
										</li>
										<li><img src="svg/emoji/027.svg" class="img-fluid blur-up lazyloaded" alt="smile">
										</li>
										<li><img src="svg/emoji/052.svg" class="img-fluid blur-up lazyloaded" alt="smile">
										</li>
										<li><img src="svg/emoji/039.svg" class="img-fluid blur-up lazyloaded" alt="smile">
										</li>
										<li><img src="svg/emoji/042.svg" class="img-fluid blur-up lazyloaded" alt="smile">
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
</div>
{/if}