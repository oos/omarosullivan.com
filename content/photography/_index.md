---
title: "Photography"
date: 2025-01-04
---

<style>
/* Force 2-column layout for photography posts - testing */
.posts-entry,
.post-entries,
.posts,
.entries {
  display: grid !important;
  grid-template-columns: repeat(2, 1fr) !important;
  gap: 15px !important;
}

.posts-entry .post-entry,
.post-entries .post-entry,
.posts .post-entry,
.entries .post-entry {
  width: 100% !important;
  margin: 0 !important;
  display: block !important;
}

/* Also target individual post entries */
.post-entry {
  display: inline-block !important;
  width: 48% !important;
  margin: 1% !important;
  vertical-align: top !important;
  box-sizing: border-box !important;
}

@media (max-width: 768px) {
  .posts-entry,
  .post-entries,
  .posts,
  .entries {
    grid-template-columns: repeat(2, 1fr) !important;
  }
  
  .post-entry {
    width: 48% !important;
  }
}

@media (max-width: 480px) {
  .posts-entry,
  .post-entries,
  .posts,
  .entries {
    grid-template-columns: 1fr !important;
  }
  
  .post-entry {
    width: 100% !important;
  }
}
</style>

