<template>
  <WelcomeItem>
    <template #icon><DocumentationIcon /></template>
    <template #heading>Blog</template>

    <p>
      Check back for short and concise articles where I share some of the most
      useful techniques and tools I've found that have helped me use Obsidian.
    </p>
  </WelcomeItem>

  <WelcomeItem>
    <template #icon><CommunityIcon /></template>
    <template #heading>Newsletter</template>

    <p>
      If you want the tips sent to your inbox, sign up for a once a month email
      that will go out at the end of each month. Your email will never be used
      for spam or shared with any third parties.
    </p>

    <form name="contact" method="POST" data-netlify="true">
      <div class="base-input-wrapper">
        <label for="name">Name: </label>
        <input type="text" name="name" style="padding: 5px" />
      </div>
      <div class="base-input-wrapper">
        <label for="email">Email: </label>
        <input type="text" name="email" style="padding: 5px" />
      </div>
      <p>
        <button type="submit" style="padding: 0.5rem">Submit</button>
      </p>
    </form>
  </WelcomeItem>
</template>

<style scoped>
.base-input-wrapper {
  display: grid;
  grid-template-columns: 50px 1fr;
  margin-top: 15px;
  margin-bottom: 15px;
}
</style>
