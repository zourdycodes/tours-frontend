// const show = document.querySelector(".navigation__show-menu");
// const bgShow = document.querySelector(".navigation__show-bg");
"use-strict";

//! popup functionality
//! remove link when clicked
const popupBtn = document.querySelectorAll("#btn-popup");
const popup = document.getElementById("popup");
const exitPopup = document.getElementById("popup-exit");
const bookBtn = document.getElementById("booking-btn");
const navLink = document.querySelectorAll(".navigation__link");
const menu = document.getElementById("nav-menu");
const bgMenu = document.getElementById("bg-menu");

const showMenu = (toggleId, navId, bgId) => {
  const toggle = document.getElementById(toggleId);
  const nav = document.getElementById(navId);
  const bg = document.getElementById(bgId);

  if (toggle && nav && bg) {
    toggle.addEventListener("click", () => {
      nav.classList.toggle("navigation__show-menu");
      bg.classList.toggle("navigation__show-bg");
    });
  }
};

showMenu("nav-toggle", "nav-menu", "bg-menu");

//! remove link when clicked

navLink.forEach((n) => {
  n.addEventListener("click", (e) => {
    menu.classList.remove("navigation__show-menu");
    bgMenu.classList.remove("navigation__show-bg");
  });
});

//! popup functionality

popupBtn.forEach((n) => {
  n.addEventListener("click", (e) => {
    e.preventDefault();
    popup.classList.remove("popup__none");
  });
});

//? Exit Popup
exitPopup.addEventListener("click", (e) => {
  e.preventDefault();
  popup.classList.add("popup__none");
});

//? Onclick to direct link it will dissapear the popup modal
bookBtn.addEventListener("click", (e) => {
  e.preventDefault();
  setTimeout(() => {
    popup.classList.add("popup__none");
  }, 2000);
});
