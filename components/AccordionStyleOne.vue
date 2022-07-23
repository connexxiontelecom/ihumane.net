<template>
  <div class="agency-accordion">
    <b-card no-body>
      <b-card-header header-tag="header" class="card-header">
        <b-button block v-b-toggle.accordion-1 class="acc-btn border-0 text-left">
          Can I run payroll for my clients using IHUMANE?
        </b-button>
      </b-card-header>
      <b-collapse id="accordion-1" visible accordion="my-accordion">
        <b-card-body>
          <b-card-text>
            Yes, IHUMANE helps HR outsourcing firms manage the payroll of their clients irrespective of their staff
            strength.
          </b-card-text>
        </b-card-body>
      </b-collapse>
    </b-card>
    <b-card no-body>
      <b-card-header header-tag="header" class="card-header">
        <b-button block v-b-toggle.accordion-2 class="acc-btn border-0 text-left">
          Can IHUMANE be customized?
        </b-button>
      </b-card-header>
      <b-collapse id="accordion-2" visible accordion="my-accordion">
        <b-card-body>
          <b-card-text>
            Yes, IHUMANE can be customized to suit your unique needs. We pride ourselves as one of the most flexible and
            customizable HRIS in the world.
          </b-card-text>
        </b-card-body>
      </b-collapse>
    </b-card>
    <b-card no-body>
      <b-card-header header-tag="header" class="card-header">
        <b-button block v-b-toggle.accordion-3 class="acc-btn border-0 text-left">
          How secure is IHUMANE?
        </b-button>
      </b-card-header>
      <b-collapse id="accordion-3" visible accordion="my-accordion">
        <b-card-body>
          <b-card-text>
            IHUMANE is designed to be secure and user-friendly. It uses an encrypted database to store employee
            information, and all data is transmitted over a secure SSL connection.
          </b-card-text>
        </b-card-body>
      </b-collapse>
    </b-card>
    <b-card no-body>
      <b-card-header header-tag="header" class="card-header">
        <b-button block v-b-toggle.accordion-4 class="acc-btn border-0 text-left">
          Can I use IHUMANE for my subsidiaries?
        </b-button>
      </b-card-header>
      <b-collapse id="accordion-4" visible accordion="my-accordion">
        <b-card-body>
          <b-card-text>
            Yes, IHUMANE has the bandwidth to manage the Human Resource activities of all your subsidiaries.
          </b-card-text>
        </b-card-body>
      </b-collapse>
    </b-card>
  </div>
</template>
