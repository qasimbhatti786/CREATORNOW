// Text Reveal Animation for Hero Title
gsap.from(".hero-title", {
  y: 50,
  opacity: 0,
  duration: 1,
  ease: "power3.out"
});

// Scroll Animations
gsap.utils.toArray(".section-title").forEach(title => {
  gsap.from(title, {
    scrollTrigger: {
      trigger: title,
      start: "top 80%"
    },
    y: 30,
    opacity: 0,
    duration: 1,
    ease: "power3.out"
  });
});
