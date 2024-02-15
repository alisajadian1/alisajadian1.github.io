<template>
  <div class="header-area header-transparent">
    <div class="main-header header-sticky">
      <div class="container">
        <div class="row align-items-center">
          <div class="col-xl-2 col-lg-2 col-md-2">
            <div class="logo">
              <img src="@/assets/logo.svg" alt="Logo" />
            </div>
          </div>
          <div class="col-xl-10 col-lg-10 col-md-10">
            <div class="main-menu float-end d-none d-lg-block">
              <nav>
                <ul id="navigation">
                  <li class="nav-item">
                    <a class="nav-link" href="#">Home</a>
                  </li>
                  <li class="nav-item">
                    <a class="nav-link" href="#">About</a>
                  </li>
                  <li class="nav-item">
                    <a class="nav-link" href="#">Resume</a>
                  </li>
                  <li class="nav-item">
                    <a class="nav-link" href="#">Contact</a>
                  </li>
                </ul>
              </nav>
            </div>
          </div>
          <div class="col-12">
            <div class="mobile-menu d-block d-lg-none">
              <div class="slicknav-menu">
                <a
                  href="#"
                  aria-haspopup="true"
                  role="button"
                  tabindex="0"
                  class="slicknav-btn slicknav-collapsed"
                  style="outline: none"
                >
                  <span class="slicknav-menutxt">Menu</span>
                  <span class="slicknav-icon">
                    <span slicknav-icon-bar></span>
                    <span slicknav-icon-bar></span>
                    <span slicknav-icon-bar></span>
                  </span>
                </a>
                <ul
                  class="slicknav-nav slicknav-hidden"
                  style="display: none"
                  aria-hidden="true"
                  role="menu"
                >
                  <li class="nav-item">
                    <a
                      href="#"
                      class="nav-link transition active"
                      role="menuitem"
                      tabindex="-1"
                      >Home</a
                    >
                  </li>
                  <li class="nav-item">
                    <a
                      href="#"
                      class="nav-link transition active"
                      role="menuitem"
                      tabindex="-1"
                      >About</a
                    >
                  </li>
                  <li class="nav-item">
                    <a
                      href="#"
                      class="nav-link transition active"
                      role="menuitem"
                      tabindex="-1"
                      >Resume</a
                    >
                  </li>
                  <li class="nav-item">
                    <a
                      href="#"
                      class="nav-link transition active"
                      role="menuitem"
                      tabindex="-1"
                      >Contact</a
                    >
                  </li>
                </ul>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style>
.header-transparent {
  position: absolute;
  top: 0;
  right: 0;
  left: 0;
  z-index: 1000;
  padding: 10px 0; /* Add padding to the header */
}

.logo img {
  margin: 0;
  padding: 0;
  border: 0;
  outline: 0;
  max-width: 50px;
  height: auto;
  vertical-align: middle;
}

.main-menu ul {
  list-style: none;
  margin: 0;
  padding: 0;
}

.main-menu li {
  display: inline-block;
  margin-right: 20px;
}

.main-menu a {
  text-decoration: none;
  color: black;
  font-weight: bold;
  transition: color 0.3s ease;
}

.main-header .main-menu ul li .nav-link:hover::before {
  width: 100%;
}

.main-header .main-menu ul li .nav-link {
  display: inline-block;
  position: relative;
  color: #222222;
  padding: 25px 16px;
  font-weight: 400;
  font-size: 16px;
  text-transform: capitalize;
}

.main-header .main-menu ul li .nav-link::before {
  display: inline-block;
  position: absolute;
  display: inline-block;
  content: "";
  left: 0;
  bottom: 14px;
  background-color: #e45447;
  height: 1px;
  width: 0px;
  transition: all 0.3s ease 0s;
}
</style>
