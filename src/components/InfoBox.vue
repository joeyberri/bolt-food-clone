<template>
  <div>
    <div class="info-box">
      <div class="box-icon">
        <svg
          xmlns="http://www.w3.org/2000/svg"
          width="24"
          height="24"
          viewBox="0 0 24 24"
        >
          <path
            d="M21 20V4a1 1 0 0 0-1-1H4a1 1 0 0 0-1 1v16a1 1 0 0 0 1 1h16a1 1 0 0 0 1-1zm-2-1H5V5h14v14z"
          />
          <path
            d="M10.381 12.309l3.172 1.586a1 1 0 0 0 1.305-.38l3-5-1.715-1.029-2.523 4.206-3.172-1.586a1.002 1.002 0 0 0-1.305.38l-3 5 1.715 1.029 2.523-4.206z"
          />
        </svg>
      </div>

      <div class="box-content">
        <span class="big">44.51</span>
        Current price ($)
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "InfoBox",
  props: {},
};
</script>
