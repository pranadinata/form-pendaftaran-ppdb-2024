<script setup lang="ts">
import Button from "@/components/Base/Button";
import { FormInput, FormLabel, FormSelect } from "@/components/Base/Form";
</script>

<template>
  <div class="flex items-center mt-8 intro-y">
    <h2 class="mr-auto text-lg font-medium">Wizard Layout</h2>
  </div>
  <!-- BEGIN: Wizard Layout -->
  <div class="py-10 mt-5 intro-y box sm:py-20">
    <div class="px-5 sm:px-20">
      <div class="flex items-center intro-x">
        <Button variant="primary" class="w-10 h-10 rounded-full"> 1 </Button>
        <div class="ml-3 text-base font-medium">Create New Account</div>
      </div>
      <div class="flex items-center mt-5 intro-x">
        <Button
          class="w-10 h-10 rounded-full text-slate-500 bg-slate-100 dark:bg-darkmode-400 dark:border-darkmode-400"
        >
          2
        </Button>
        <div class="ml-3 text-base text-slate-600 dark:text-slate-500">
          Setup Your Profile
        </div>
      </div>
      <div class="flex items-center mt-5 intro-x">
        <Button
          class="w-10 h-10 rounded-full text-slate-500 bg-slate-100 dark:bg-darkmode-400 dark:border-darkmode-400"
        >
          3
        </Button>
        <div class="ml-3 text-base text-slate-600 dark:text-slate-500">
          Setup Your Business Details
        </div>
      </div>
      <div class="flex items-center mt-5 intro-x">
        <Button
          class="w-10 h-10 rounded-full text-slate-500 bg-slate-100 dark:bg-darkmode-400 dark:border-darkmode-400"
        >
          4
        </Button>
        <div class="ml-3 text-base text-slate-600 dark:text-slate-500">
          Setup Billing Account
        </div>
      </div>
      <div class="flex items-center mt-5 intro-x">
        <Button
          class="w-10 h-10 rounded-full text-slate-500 bg-slate-100 dark:bg-darkmode-400 dark:border-darkmode-400"
        >
          5
        </Button>
        <div class="ml-3 text-base text-slate-600 dark:text-slate-500">
          Finalize your purchase
        </div>
      </div>
    </div>
    <div
      class="px-5 pt-10 mt-10 border-t sm:px-20 border-slate-200/60 dark:border-darkmode-400"
    >
      <div class="text-base font-medium">Profile Settings</div>
      <div class="grid grid-cols-12 gap-4 mt-5 gap-y-5">
        <div class="col-span-12 intro-y sm:col-span-6">
          <FormLabel htmlFor="input-wizard-1">From</FormLabel>
          <FormInput
            id="input-wizard-1"
            type="text"
            placeholder="example@gmail.com"
          />
        </div>
        <div class="col-span-12 intro-y sm:col-span-6">
          <FormLabel htmlFor="input-wizard-2">To</FormLabel>
          <FormInput
            id="input-wizard-2"
            type="text"
            placeholder="example@gmail.com"
          />
        </div>
        <div class="col-span-12 intro-y sm:col-span-6">
          <FormLabel htmlFor="input-wizard-3">Subject</FormLabel>
          <FormInput
            id="input-wizard-3"
            type="text"
            placeholder="Important Meeting"
          />
        </div>
        <div class="col-span-12 intro-y sm:col-span-6">
          <FormLabel htmlFor="input-wizard-4">Has the Words</FormLabel>
          <FormInput
            id="input-wizard-4"
            type="text"
            placeholder="Job, Work, Documentation"
          />
        </div>
        <div class="col-span-12 intro-y sm:col-span-6">
          <FormLabel htmlFor="input-wizard-5">Doesn't Have</FormLabel>
          <FormInput
            id="input-wizard-5"
            type="text"
            placeholder="Job, Work, Documentation"
          />
        </div>
        <div class="col-span-12 intro-y sm:col-span-6">
          <FormLabel htmlFor="input-wizard-6">Size</FormLabel>
          <FormSelect id="input-wizard-6">
            <option>10</option>
            <option>25</option>
            <option>35</option>
            <option>50</option>
          </FormSelect>
        </div>
        <div
          class="flex items-center justify-center col-span-12 mt-5 intro-y sm:justify-end"
        >
          <Button variant="secondary" class="w-24"> Previous </Button>
          <Button variant="primary" class="w-24 ml-2"> Next </Button>
        </div>
      </div>
    </div>
  </div>
  <!-- END: Wizard Layout -->
</template>
