<template>
  <div class="relative bg-white">
    <div class="absolute inset-0">
      <div class="absolute inset-y-0 left-0 w-1/2 bg-gray-50" />
    </div>
    <div class="relative mx-auto max-w-7xl lg:grid lg:grid-cols-5">
      <div
        class="px-4 py-16 bg-gray-50 sm:px-6 lg:col-span-2 lg:px-8 lg:py-24 xl:pr-12"
      >
        <div class="max-w-lg mx-auto">
          <h2
            class="text-2xl font-extrabold tracking-tight text-gray-900 sm:text-3xl"
          >
            Get in touch
          </h2>
          <p class="mt-3 text-lg leading-6 text-gray-500">
            Nullam risus blandit ac aliquam justo ipsum. Quam mauris volutpat
            massa dictumst amet. Sapien tortor lacus arcu.
          </p>
          <dl class="mt-8 text-base text-gray-500">
            <div>
              <dt class="sr-only">Postal address</dt>
              <dd>
                <p>742 Evergreen Terrace</p>
                <p>Springfield, OR 12345</p>
              </dd>
            </div>
            <div class="mt-6">
              <dt class="sr-only">Phone number</dt>
              <dd class="flex">
                <PhoneIcon
                  class="flex-shrink-0 w-6 h-6 text-gray-400"
                  aria-hidden="true"
                />
                <span class="ml-3"> +1 (555) 123-4567 </span>
              </dd>
            </div>
            <div class="mt-3">
              <dt class="sr-only">Email</dt>
              <dd class="flex">
                <MailIcon
                  class="flex-shrink-0 w-6 h-6 text-gray-400"
                  aria-hidden="true"
                />
                <span class="ml-3"> support@example.com </span>
              </dd>
            </div>
          </dl>
          <p class="mt-6 text-base text-gray-500">
            Looking for careers?
            {{ " " }}
            <a href="#" class="font-medium text-gray-700 underline"
              >View all job openings</a
            >.
          </p>
        </div>
      </div>
      <div
        class="px-4 py-16 bg-white sm:px-6 lg:col-span-3 lg:py-24 lg:px-8 xl:pl-12"
      >
        <div class="max-w-lg mx-auto lg:max-w-none">
          <form
            netlify
            action="https://formspree.io/f/xrgjejpe"
            netlify-honeypot="bot-field"
            name="contact"
            method="POST"
            class="grid grid-cols-1 gap-y-6"
          >
            <input type="hidden" name="form-name" value="contact" />
            <input type="hidden" name="_language" value="pl" />
            <div>
              <label for="full-name" class="sr-only">Full name</label>
              <input
                type="text"
                name="full-name"
                id="full-name"
                autocomplete="name"
                class="block w-full px-4 py-3 placeholder-gray-500 border-gray-300 rounded-md shadow-sm focus:ring-indigo-500 focus:border-indigo-500"
                placeholder="Full name"
              />
            </div>
            <div>
              <label for="email" class="sr-only">Email</label>
              <input
                id="email"
                name="email"
                type="email"
                autocomplete="email"
                class="block w-full px-4 py-3 placeholder-gray-500 border-gray-300 rounded-md shadow-sm focus:ring-indigo-500 focus:border-indigo-500"
                placeholder="Email"
              />
            </div>
            <div>
              <label for="phone" class="sr-only">Phone</label>
              <input
                type="text"
                name="phone"
                id="phone"
                autocomplete="tel"
                class="block w-full px-4 py-3 placeholder-gray-500 border-gray-300 rounded-md shadow-sm focus:ring-indigo-500 focus:border-indigo-500"
                placeholder="Phone"
              />
            </div>
            <div>
              <label for="message" class="sr-only">Message</label>
              <textarea
                id="message"
                name="message"
                rows="4"
                class="block w-full px-4 py-3 placeholder-gray-500 border border-gray-300 rounded-md shadow-sm focus:ring-indigo-500 focus:border-indigo-500"
                placeholder="Message"
              />
            </div>
            <div>
              <button
                type="submit"
                class="inline-flex justify-center px-6 py-3 text-base font-medium text-white bg-indigo-600 border border-transparent rounded-md shadow-sm hover:bg-indigo-700 focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-indigo-500"
              >
                Submit
              </button>
            </div>
          </form>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import { MailIcon, PhoneIcon } from "@heroicons/vue/outline";

export default {
  components: {
    MailIcon,
    PhoneIcon,
  },
};
</script>
