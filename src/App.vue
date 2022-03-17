<script setup></script>

<template>
  <div class="flex-column flex min-h-screen sm:overflow-hidden">
    <div class="fixed top-0 left-0 z-10 h-screen w-64 shrink-0 -translate-x-full overflow-hidden border-r border-slate-200 bg-white pb-20 pt-24 transition-all duration-300 ease-in md:w-24 md:translate-x-0 lg:w-64 xl:pt-36">
      <div class="justify absolute inset-0 flex h-24 items-center justify-center xl:h-36">
        <button class="relative -top-1 mr-6 hidden">
          <svg class="icon icon-close">
            <use xlink:href="./assets/img/sprite.svg#icon-close"></use>
          </svg>
        </button>
        <a class="opacity-100 transition-opacity duration-200 md:opacity-0 lg:opacity-100" href="index.html">
          <img class="w-36" src="./assets/img/logo.png" alt="" />
          <img class="hidden" src="./assets/img/logo-white.png" alt="" />
        </a>
        <button class="sidebar__burger"></button>
      </div>
      <div class="hide-scrollbar max-h-full overflow-y-auto px-5 pb-8">
        <div class="sidebar__inner">
          <a class="-mx-5 flex h-20 items-center justify-center lg:hidden" href="index.html">
            <img class="w-36" src="./assets/img/logo-sm.png" alt="" />
          </a>
          <div class="mb-0md:mb-5">
            <div class="mb-5 border-b border-slate-200 pb-4 last:mb-0 last:pb-0 md:mb-10 md:pb-8">
              <div class="sidebar__caption caption-sm">Admin<span> tools</span></div>
              <div class="sidebar__menu">
                <a class="sidebar__item active" href="index.html">
                  <div class="sidebar__icon">
                    <svg class="icon icon-overview">
                      <use xlink:href="./assets/img/sprite.svg#icon-overview"></use>
                    </svg>
                  </div>
                  <div class="sidebar__text">Overview</div> </a
                ><a class="sidebar__item" href="products.html">
                  <div class="sidebar__icon">
                    <svg class="icon icon-bag">
                      <use xlink:href="./assets/img/sprite.svg#icon-bag"></use>
                    </svg>
                  </div>
                  <div class="sidebar__text">Products</div> </a
                ><a class="sidebar__item" href="campaigns.html">
                  <div class="sidebar__icon">
                    <svg class="icon icon-chart">
                      <use xlink:href="./assets/img/sprite.svg#icon-chart"></use>
                    </svg>
                  </div>
                  <div class="sidebar__text">Campaigns</div> </a
                ><a class="sidebar__item" href="schedules.html">
                  <div class="sidebar__icon">
                    <svg class="icon icon-discovery">
                      <use xlink:href="./assets/img/sprite.svg#icon-discovery"></use>
                    </svg>
                  </div>
                  <div class="sidebar__text">Schedules</div> </a
                ><a class="sidebar__item" href="payouts.html">
                  <div class="sidebar__icon">
                    <svg class="icon icon-wallet">
                      <use xlink:href="./assets/img/sprite.svg#icon-wallet"></use>
                    </svg>
                  </div>
                  <div class="sidebar__text">Payouts</div> </a
                ><a class="sidebar__item" href="statement.html">
                  <div class="sidebar__icon">
                    <svg class="icon icon-document">
                      <use xlink:href="./assets/img/sprite.svg#icon-document"></use>
                    </svg>
                  </div>
                  <div class="sidebar__text">Statements</div> </a
                ><a class="sidebar__item js-popup-open" href="#popup-settings" data-effect="mfp-zoom-in">
                  <div class="sidebar__icon">
                    <svg class="icon icon-settings">
                      <use xlink:href="./assets/img/sprite.svg#icon-settings"></use>
                    </svg>
                  </div>
                  <div class="sidebar__text">Settings</div>
                </a>
              </div>
            </div>
            <div class="sidebar__group">
              <div class="sidebar__caption caption-sm">Insights</div>
              <div class="sidebar__menu">
                <a class="sidebar__item" href="inbox.html">
                  <div class="sidebar__icon">
                    <svg class="icon icon-message">
                      <use xlink:href="./assets/img/sprite.svg#icon-message"></use>
                    </svg>
                  </div>
                  <div class="sidebar__text">Inbox</div>
                  <div class="sidebar__counter">18</div> </a
                ><a class="sidebar__item" href="notifications.html">
                  <div class="sidebar__icon">
                    <svg class="icon icon-notification">
                      <use xlink:href="./assets/img/sprite.svg#icon-notification"></use>
                    </svg>
                  </div>
                  <div class="sidebar__text">Notifications</div>
                  <div class="sidebar__counter">2</div> </a
                ><a class="sidebar__item" href="comments.html">
                  <div class="sidebar__icon">
                    <svg class="icon icon-chat">
                      <use xlink:href="./assets/img/sprite.svg#icon-chat"></use>
                    </svg>
                  </div>
                  <div class="sidebar__text">Comments</div>
                  <div class="sidebar__counter">20</div>
                </a>
              </div>
            </div>
          </div>
          <div class="sidebar__profile">
            <div class="sidebar__details">
              <a class="sidebar__link" href="#">
                <div class="sidebar__icon">
                  <svg class="icon icon-profile">
                    <use xlink:href="./assets/img/sprite.svg#icon-profile"></use>
                  </svg>
                </div>
                <div class="sidebar__text">Profile</div> </a
              ><a class="sidebar__link" href="#">
                <div class="sidebar__icon">
                  <svg class="icon icon-logout">
                    <use xlink:href="./assets/img/sprite.svg#icon-logout"></use>
                  </svg>
                </div>
                <div class="sidebar__text">Log out</div>
              </a>
            </div>
            <a class="sidebar__user" href="#">
              <div class="sidebar__ava">
                <img class="sidebar__pic" src="./assets/img/ava.png" alt="" />
              </div>
              <div class="sidebar__desc">
                <div class="sidebar__man">Tam Tran</div>
                <div class="sidebar__status caption">Free account</div>
              </div>
              <div class="sidebar__arrow">
                <svg class="icon icon-arrows">
                  <use xlink:href="./assets/img/sprite.svg#icon-arrows"></use>
                </svg>
              </div>
            </a>
          </div>
        </div>
      </div>
      <div class="sidebar__bottom">
        <label class="switch switch_theme js-switch-theme"
          ><input class="switch__input" type="checkbox" /><span class="switch__in"
            ><span class="switch__box"></span
            ><span class="switch__icon"
              ><svg class="icon icon-moon">
                <use xlink:href="./assets/img/sprite.svg#icon-moon"></use></svg
              ><svg class="icon icon-sun">
                <use xlink:href="./assets/img/sprite.svg#icon-sun"></use></svg></span></span
        ></label>
      </div>
    </div>
    <div class="page__wrapper">
      <div class="page__center">
        <div class="page__row page__row_head page__row_border">
          <div class="page__col">
            <div class="page__hello h5">Hi Tam Tran,</div>
            <div class="page__welcome h2">Welcome back<span class="desktop-hide">👋</span></div>
          </div>
          <div class="page__col">
            <div class="header">
              <button class="header__burger"></button>
              <div class="search">
                <div class="search__field">
                  <input class="search__input" type="text" placeholder="Search" /><button class="search__toggle">
                    <svg class="icon icon-search">
                      <use xlink:href="./assets/img/sprite.svg#icon-search"></use></svg
                    ><svg class="icon icon-close">
                      <use xlink:href="./assets/img/sprite.svg#icon-close"></use>
                    </svg>
                  </button>
                </div>
                <div class="search__result">
                  <div class="search__info caption-sm">Recent Searches</div>
                  <div class="search__list">
                    <a class="search__item" href="#">
                      <div class="search__preview bg-pink">
                        <img class="search__pic" src="./assets/img/figure-1.png" alt="" />
                      </div>
                      <div class="search__text">
                        Earning byitems<svg class="icon icon-arrow-right">
                          <use xlink:href="./assets/img/sprite.svg#icon-arrow-right"></use>
                        </svg>
                      </div>
                    </a>
                    <a class="search__item" href="#">
                      <div class="search__preview bg-yellow">
                        <img class="search__pic" src="./assets/img/figure-4.png" alt="" />
                      </div>
                      <div class="search__text">
                        This monthStatements<svg class="icon icon-arrow-right">
                          <use xlink:href="./assets/img/sprite.svg#icon-arrow-right"></use>
                        </svg>
                      </div> </a
                    ><a class="search__item" href="#">
                      <div class="search__preview bg-blue-light">
                        <img class="search__pic" src="./assets/img/figure-3.png" alt="" />
                      </div>
                      <div class="search__text">
                        How manysales I got…<svg class="icon icon-arrow-right">
                          <use xlink:href="./assets/img/sprite.svg#icon-arrow-right"></use>
                        </svg>
                      </div>
                    </a>
                  </div>
                  <button class="search__btn btn btn_purple btn_wide">Advance Search</button>
                </div>
              </div>
              <button class="header__search">
                <svg class="icon icon-search">
                  <use xlink:href="./assets/img/sprite.svg#icon-search"></use>
                </svg>
              </button>
              <div class="notifications">
                <button class="notifications__open">
                  <svg class="icon icon-bell">
                    <use xlink:href="./assets/img/sprite.svg#icon-bell"></use></svg
                  ><span class="notifications__counter">2</span>
                </button>
                <div class="notifications__wrap">
                  <div class="notifications__info h6">Recent Notification</div>
                  <div class="notifications__list">
                    <a class="notifications__item" href="notifications.html">
                      <div class="notifications__ava">
                        <img class="notifications__pic" src="./assets/img/ava-1.png" alt="" />
                        <div class="notifications__status bg-blue">
                          <img class="notifications__pic" src="./assets/img/chat.svg" alt="" />
                        </div>
                      </div>
                      <div class="notifications__details">
                        <div class="notifications__line">
                          <div class="notifications__user caption">Sarah Saunders</div>
                          <div class="notifications__time caption">8h</div>
                        </div>
                        <div class="notifications__text caption-sm">
                          Commented on
                          <span class="notifications__project">Collab Design</span>
                        </div>
                      </div> </a
                    ><a class="notifications__item" href="notifications.html">
                      <div class="notifications__ava">
                        <img class="notifications__pic" src="./assets/img/ava-1.png" alt="" />
                        <div class="notifications__status bg-green">
                          <img class="notifications__pic" src="./assets/img/bag.svg" alt="" />
                        </div>
                      </div>
                      <div class="notifications__details">
                        <div class="notifications__line">
                          <div class="notifications__user caption">Glenn Greer</div>
                          <div class="notifications__time caption">12h</div>
                        </div>
                        <div class="notifications__text caption-sm">
                          Just pushaded
                          <span class="notifications__project">Sapiens Illustration</span>
                        </div>
                      </div> </a
                    ><a class="notifications__item" href="notifications.html">
                      <div class="notifications__ava">
                        <img class="notifications__pic" src="./assets/img/ava-1.png" alt="" />
                        <div class="notifications__status bg-purple">
                          <img class="notifications__pic" src="./assets/img/message.svg" alt="" />
                        </div>
                      </div>
                      <div class="notifications__details">
                        <div class="notifications__line">
                          <div class="notifications__user caption">Sarah Saunders</div>
                          <div class="notifications__time caption">14h</div>
                        </div>
                        <div class="notifications__text caption-sm">Sent you a message 📪</div>
                      </div> </a
                    ><a class="notifications__item" href="notifications.html">
                      <div class="notifications__ava">
                        <img class="notifications__pic" src="./assets/img/ava-1.png" alt="" />
                        <div class="notifications__status bg-red">
                          <img class="notifications__pic" src="./assets/img/heart.svg" alt="" />
                        </div>
                      </div>
                      <div class="notifications__details">
                        <div class="notifications__line">
                          <div class="notifications__user caption">Sarah Saunders</div>
                          <div class="notifications__time caption">21h</div>
                        </div>
                        <div class="notifications__text caption-sm">
                          Liked
                          <span class="notifications__project">Folio Agency</span>
                        </div>
                      </div> </a
                    ><a class="notifications__item" href="notifications.html">
                      <div class="notifications__ava">
                        <img class="notifications__pic" src="./assets/img/ava-1.png" alt="" />
                        <div class="notifications__status bg-blue">
                          <img class="notifications__pic" src="./assets/img/chat.svg" alt="" />
                        </div>
                      </div>
                      <div class="notifications__details">
                        <div class="notifications__line">
                          <div class="notifications__user caption">Sarah Saunders</div>
                          <div class="notifications__time caption">8h</div>
                        </div>
                        <div class="notifications__text caption-sm">
                          Commented on
                          <span class="notifications__project">Collab Design</span>
                        </div>
                      </div> </a
                    ><a class="notifications__item" href="notifications.html">
                      <div class="notifications__ava">
                        <img class="notifications__pic" src="./assets/img/ava-1.png" alt="" />
                        <div class="notifications__status bg-green">
                          <img class="notifications__pic" src="./assets/img/bag.svg" alt="" />
                        </div>
                      </div>
                      <div class="notifications__details">
                        <div class="notifications__line">
                          <div class="notifications__user caption">Glenn Greer</div>
                          <div class="notifications__time caption">12h</div>
                        </div>
                        <div class="notifications__text caption-sm">
                          Just pushaded
                          <span class="notifications__project">Sapiens Illustration</span>
                        </div>
                      </div>
                    </a>
                  </div>
                  <div class="notifications__btns">
                    <a class="notifications__btn btn btn_black" href="notifications.html">See all incoming activity</a>
                  </div>
                </div>
              </div>
              <a class="header__user" href="#"><img class="header__pic" src="./assets/img/ava.png" alt="" /></a>
            </div>
          </div>
        </div>
        <div class="page__row page__row_border">
          <div class="page__col"></div>
          <div class="page__col">
            <div class="page__group"></div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
