<template>
  <form
    name="contactUs"
    method="POST"
    data-netlify="true"
    netlify-honeypot="bot-field"
  >
    <input type="hidden" name="form-name" value="contactUs" />
    <p class="hidden">
      <label>
        Don’t fill this out if you're human: <input name="bot-field" />
      </label>
    </p>
    <div class="field">
      <label class="label is-medium">Name</label>
      <div class="control has-icons-left">
        <input name="name" class="input is-medium" type="text" placeholder="" />
        <span class="icon is-small is-left">
          <font-awesome-icon icon="user" />
        </span>
      </div>
    </div>
    <!-- Email -->
    <div class="field">
      <label class="label is-medium">Email</label>
      <div class="control has-icons-left">
        <input
          name="email"
          class="input is-medium"
          type="email"
          placeholder=""
        />
        <span class="icon is-small is-left">
          <font-awesome-icon icon="envelope" />
        </span>
      </div>
    </div>
    <!-- Message -->
    <div class="field">
      <label class="label is-medium">Message</label>
      <div class="control">
        <textarea
          name="message"
          class="textarea"
          placeholder="Detailed description of your comment, request, etc"
          rows="8"
        ></textarea>
      </div>
    </div>
    <div class="control">
      <button class="button is-primary">
        Contact Us
      </button>
    </div>
  </form>
</template>
<style>
.hidden {
  visibility: hidden;
}
</style>
