<template>
  <div>
    <div class="bloсk_benefits">
      <div class="conteiner_benefits">
        <div class="cells_benefits">
          <div class="cells_benefits_icon">
            <svg
              width="83"
              height="83"
              viewBox="0 0 83 83"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
              xmlns:xlink="http://www.w3.org/1999/xlink"
            >
              <path
                d="M0 41.5C0 18.5802 18.5802 0 41.5 0C64.4198 0 83 18.5802 83 41.5C83 64.4198 64.4198 83 41.5 83C18.5802 83 0 64.4198 0 41.5Z"
                fill="#292E36"
              />
              <path d="M68 15H16V67H68V15Z" fill="url(#pattern0)" />
              <defs>
                <pattern
                  id="pattern0"
                  patternContentUnits="objectBoundingBox"
                  width="1"
                  height="1"
                >
                  <use xlink:href="#image0_2_110" transform="scale(0.01)" />
                </pattern>
                <image
                  id="image0_2_110"
                  width="100"
                  height="100"
                  xlink:href="data:image/png;base64,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"
                />
              </defs>
            </svg>
          </div>
          <div class="cells_benefits_text">
            <span class="cells_benefits_span"> Locate Us </span>
            <p class="cells_benefits_p">Riverside 25, San Diego, California</p>
          </div>
        </div>
        <div class="cells_benefits">
          <div class="cells_benefits_icon">
            <svg
              width="83"
              height="83"
              viewBox="0 0 83 83"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                d="M0 41.5C0 18.5802 18.5802 0 41.5 0C64.4198 0 83 18.5802 83 41.5C83 64.4198 64.4198 83 41.5 83C18.5802 83 0 64.4198 0 41.5Z"
                fill="#292E36"
              />
              <path
                d="M25.117 26.8067C21.5545 30.792 19.5619 35.9245 19.5015 41.2582C19.3606 53.4554 29.3237 63.4588 41.5007 63.499C53.6778 63.5191 63.5 53.6567 63.5 41.4997C63.5 29.5239 53.9193 19.7621 42.0039 19.5005C41.9435 19.5005 41.863 19.5005 41.8026 19.5407C41.7423 19.5609 41.6819 19.6011 41.6416 19.6414C41.6014 19.6816 41.5611 19.742 41.5209 19.8024C41.5007 19.8628 41.4806 19.9232 41.4806 20.0037V29.5843"
                stroke="white"
                stroke-width="3.5"
                stroke-linecap="round"
                stroke-linejoin="round"
              />
              <path
                d="M38.9244 44.0762L29.8671 31.1342C29.7262 30.9531 29.6859 30.7317 29.706 30.5103C29.7262 30.2889 29.8067 30.0876 29.9677 29.9266C30.1287 29.7656 30.33 29.6851 30.5514 29.6649C30.7527 29.6448 30.9741 29.7052 31.1552 29.826L44.0971 38.8833C44.8821 39.4469 45.4255 40.3123 45.5866 41.2785C45.7476 42.2446 45.5262 43.2308 44.9626 44.0359C44.399 44.841 43.5537 45.3845 42.5876 45.5656C41.6215 45.7467 40.6352 45.5253 39.8301 44.9819C39.488 44.7404 39.1659 44.4385 38.9244 44.0762Z"
                fill="white"
              />
            </svg>
          </div>
          <div class="cells_benefits_text">
            <span class="cells_benefits_span"> Open Hours </span>
            <p class="cells_benefits_p">Mon To Fri 9:00 AM - 9:00 PM</p>
          </div>
        </div>
        <div class="cells_benefits">
          <div class="cells_benefits_icon">
            <svg
              width="83"
              height="83"
              viewBox="0 0 83 83"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
              xmlns:xlink="http://www.w3.org/1999/xlink"
            >
              <path
                d="M0 41.5C0 18.5802 18.5802 0 41.5 0C64.4198 0 83 18.5802 83 41.5C83 64.4198 64.4198 83 41.5 83C18.5802 83 0 64.4198 0 41.5Z"
                fill="#292E36"
              />
              <path
                d="M60.875 22.125H22.125V60.875H60.875V22.125Z"
                fill="url(#pattern0)"
              />
              <defs>
                <pattern
                  id="pattern0"
                  patternContentUnits="objectBoundingBox"
                  width="1"
                  height="1"
                >
                  <use
                    xlink:href="#image0_2_127"
                    transform="scale(0.0104167)"
                  />
                </pattern>
                <image
                  id="image0_2_127"
                  width="96"
                  height="96"
                  xlink:href="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAGAAAABgCAYAAADimHc4AAAAAXNSR0IArs4c6QAABWFJREFUeF7tncuO3EQUhv/f5RlAXF6ATTZsEsEjsAAmEBAINmHBbQEShGsQCCEIAsJNCBExgkggsuUihLgsAAFPARpgwYY3QCICMbHdB3niDj093V11qtzt7vHp7Zy/TtX/1Tkue9Rtwj6dOsBOs1tyGICON4EBMAAdO9BxeqsAA9CxAx2ntwpYdQAi24cwyB4Asw1ADgC4tOM1zTv93wD/gAx+QJafIflrSsLoChCRdQyqt0EcA+BSJrHC2goip5HlT5MsYtYRBWDHfKm+AXBDTNJ9qPkRdLfEQIgDUJXvgnh0HxoZvySRTbq149oB1AB2er64n3rcdqZ5XILuGpK/aSDoAVTFOyCf0CTpTazIKbq1pzTr1QMYFL8APKhJ0p9YbjFzV2vWGwGgPAvgMk2SHsWeZZZfoVlvDACZlYBZrh5TM+GuY2VQtrp+tVltT6BrQ7X5216/AVASMABKw9oONwBtO6oczwAoDWs73AC07ahyPAOgNKzt8JUHkLoAnz7VcN99jC+/Tz8+v4UfQ1MX4NMbAM+dsM9A3w7y6Q2AAVB1FVVwvbt8OzB1B6fqrQKsAlSbWhVsFZDeAewU5OlRqS3Qp+8cQGqP7lqfeg00AIkEDUCigalyA5DqYKLeACQamCo3AKkOJuoNQKKBqXIDkOpgon7lAaQuwKdP9Be+Gylffp++8/uA1AX49AbAHsapnq+pgu1hnD2M8/4/wlqQtSBVV1EFWwuyFmQtyHcM1J6DU3v2ovVtr3/hLWjRhrWdzwC07ahyPBmU5axviGo7gFWAFoCURyH4CEA+SWoAlIbGhMsMCAYgxtEIzTQIBiDCzFjJJAgGINbNSN04hKUHkHqMm7e+4VCBuI/M64ut9zMKwQAkPosacTsKArN8zUtsJGDhx9B572DfDvTlHzOvBHEXmX8WYqpIWccGVc1wPAPgd7auhHvJ/GN/qD7CAIR5NjcIBiAMQB1VQ7iHzD8Jl/gjDYDfo9GI1iEYAB2AYSXcTeaf6qV7FQsH0MakU8ZQnoKmpaoroRUIfQTwD4BLUiA22gLEnWT+ZcpY/QMgxbUQftvSL/wmQ+gdgHq3SvsQjpL5VzGV0EsADYQNCL9usR1FQegtgGWB0GsAywCh9wDmAOEciLod1e3N+zEAjUUixeHmmnCx1zV/QDAEAzBipkhxE4T1uT4dguA9uvwxHysDMOZQK5UgOIPMPUhyYAB8Dkz4u0hxI4T1uV5fCQrz69RWAVMAiZQ3Q/AFgIuCGQo+QOaOkdzz+9IichXJ38fHMgAz3FVVwoydL1I9A5FXJp2ODIBnewddmP3mv9mk2XM6MgAB/WUmhHDzh5l2QYgB8BeAywPmvfwh5AnSvRYy0YkQBB8icw9NOu00bWe488dTXIAQAaDaAuRQyKRXIoZ8lnTTjNq1BJHyVgg+B7AOwfvI3MOTL7jViZ2eP/tzDpQjegBVcQrkkythbugkyedI90ZIuEh5GwZyPbL8eIL5TSpu6QGIHIRUP++711iRz5Pu9RAI02JEgnb+qPxPNYBaLVWxCfLxlMkupVZxTRiff4T5gOB0HACRteZVhhtLaWTKpMgXSPeqZogo84HvQHdHFICdKqghDMq3QD4y7es6mkUsVSz5IulOhsypvsOF1AcTrIfENzHnzSe3owEMk0l9TRiU94PZ4eZ1tvvjHWPkS6R7OcTUXacjv+CC+XVoMgB/vn5EiJRHmmdHsx7gfQ+620n+O3TFALS4PzwQ9phvFdCi+f+35ImVMNF8AzAHAOcPKMV1kGwTkCt3vlOcufqN29uT0lkLmhOE0GENQKhTc4ozAHMyNnRYAxDq1Jzi/gManxMcXuh+VwAAAABJRU5ErkJggg=="
                />
              </defs>
            </svg>
          </div>
          <div class="cells_benefits_text">
            <span class="cells_benefits_span"> Reservation </span>
            <p class="cells_benefits_p email">restaurantate@gmail.com</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Benefits",
};
</script>

<style scoped>
.bloсk_benefits {
  height: auto;
  width: auto;
  background-color: rgba(255, 248, 245, 1);
}
.conteiner_benefits {
  display: flex;
  justify-content: space-around;
}
.cells_benefits {
  display: flex;
  padding: 20px;
  text-align: center;
}
.cells_benefits_icon {
  text-align: center;
}
.cells_benefits_text {
  display: flex;
  flex-direction: column;
  padding-left: 20px;
}
.cells_benefits_span {
  margin-top: 20px;
  font-weight: 900;
  text-align: center;
}
.cells_benefits_p {
  word-break: break-word;
  margin-top: 5px;
}

@media (max-width: 768px) {
  .conteiner_benefits {
    flex-direction: column;
  }
  .cells_benefits_text {
    display: flex;
    text-align: center;
  }
}
@media (max-width: 426px) {
  .cells_benefits {
    flex-direction: column;
  }
  .cells_benefits_text {
    padding-left: 0;
  }
  .cells_benefits {
    text-align: center;
  }
}
@media (min-width: 1441px) {
  .cells_benefits {
    margin-left: 150px;
  }
}
</style>
