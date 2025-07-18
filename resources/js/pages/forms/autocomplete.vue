<script setup>
import {
  asyncItems,
  basic,
  chips,
  clearable,
  customFilter,
  density,
  multiple,
  slots,
  stateSelector,
  validation,
  variant,
} from '@/views/demos/forms/form-elements/autocomplete/demoCodeAutocomplete'
</script>

<template>
  <VRow class="match-height">
    <VCol
      cols="12"
      md="6"
    >
      <!-- 👉 Basic -->
      <AppCardCode
        title="Basic"
        :code="basic"
      >
        <p>
          The <code> v-autocomplete </code> component offers simple and flexible type-ahead functionality. This is useful when searching large sets of data or even dynamically fetching information from an API.
        </p>

        <DemoAutocompleteBasic />
      </AppCardCode>
    </VCol>

    <VCol
      cols="12"
      md="6"
    >
      <!-- 👉 Density -->
      <AppCardCode
        title="Density"
        :code="density"
      >
        <p>
          You can use <code> density </code> prop to adjusts vertical spacing within the component. Available options are: <code>default</code>, <code>comfortable</code>, and <code>compact</code>.
        </p>

        <DemoAutocompleteDensity />
      </AppCardCode>
    </VCol>

    <VCol
      cols="12"
      md="12"
    >
      <!-- 👉 Variant -->
      <AppCardCode
        title="Variant"
        :code="variant"
      >
        <p>Use <code>Solo</code>, <code>Outlined</code>, <code>Underlined</code>, <code>Filled</code> and <code>Plain</code> options of <code>variant</code> prop to change the look of Autocomplete. </p>

        <DemoAutocompleteVariant />
      </AppCardCode>
    </VCol>

    <VCol
      cols="12"
      md="6"
    >
      <!-- 👉 Multiple Select -->
      <AppCardCode
        title="Multiple"
        :code="multiple"
      >
        <p>Use <code>multiple</code> prop to select multiple. Accepts array for value</p>

        <DemoAutocompleteMultiple />
      </AppCardCode>
    </VCol>

    <VCol
      cols="12"
      md="6"
    >
      <!-- 👉 Clearable input -->
      <AppCardCode
        title="Clearable"
        :code="clearable"
      >
        <p>Use <code>clearable</code> prop to add input clear functionality.</p>

        <DemoAutocompleteClearable />
      </AppCardCode>
    </VCol>

    <VCol
      cols="12"
      md="6"
    >
      <!-- 👉 Chips -->
      <AppCardCode
        title="Chips"
        :code="chips"
      >
        <p>Use <code> chips </code>  prop to use chips in select.</p>

        <DemoAutocompleteChips />
      </AppCardCode>
    </VCol>

    <VCol
      cols="12"
      md="6"
    >
      <!-- 👉 Custom Filter -->
      <AppCardCode
        title="Custom-Filter"
        :code="customFilter"
      >
        <p>The <code> custom-filter </code> prop can be used to filter each individual item with custom logic.In example we will filter state based on their name and abbreviations </p>

        <DemoAutocompleteCustomFilter />
      </AppCardCode>
    </VCol>

    <VCol
      cols="12"
      md="6"
    >
      <!-- 👉 With slots -->
      <AppCardCode
        title="Slots"
        :code="slots"
      >
        <p>With the power of slots, you can customize the visual output of the select. In this example we add a profile picture for both the chips and list items using their props. </p>

        <DemoAutocompleteSlots />
      </AppCardCode>
    </VCol>

    <VCol
      cols="12"
      md="6"
    >
      <!-- 👉 Asynchronous Items -->
      <AppCardCode
        title="Async items"
        :code="asyncItems"
      >
        <p>Sometimes you need to load data externally based upon a search query. </p>

        <DemoAutocompleteAsyncItems />
      </AppCardCode>
    </VCol>

    <VCol
      cols="12"
      md="6"
    >
      <!-- 👉 State Selector -->
      <AppCardCode
        title="State Selector"
        :code="stateSelector"
      >
        <p>Using a combination of v-autocomplete slots and transitions, you can create a stylish toggle able autocomplete field such as below state selector.</p>

        <DemoAutocompleteStateSelector />
      </AppCardCode>
    </VCol>

    <VCol
      cols="12"
      md="6"
    >
      <!-- 👉 Validation -->
      <AppCardCode
        title="validation"
        :code="validation"
      >
        <p>Use <code>rules</code>  prop to validate autocomplete. Accepts a mixed array of types function, boolean and string. Functions pass an input value as an argument and must return either true / false or a string containing an error message.</p>

        <DemoAutocompleteValidation />
      </AppCardCode>
    </VCol>
  </VRow>
</template>
