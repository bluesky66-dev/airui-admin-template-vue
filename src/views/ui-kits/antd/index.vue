<template>
  <div>
    <div class="air__utils__heading">
      <h5>
        <span class="mr-3">Ant Design Components</span>
        <a
          href="https://vue.ant.design/docs/vue/introduce/"
          rel="noopener noreferrer"
          target="_blank"
          class="btn btn-sm btn-light"
        >
          Official Documentation
          <i class="fe fe-corner-right-up" />
        </a>
      </h5>
    </div>
    <div class="row">
      <div class="col-lg-12" v-for="(category, index) in data" :key="index">
        <div class="card">
          <div class="card-body">
            <h4 class="mb-3">
              <strong>{{category.name}}</strong>
            </h4>
            <div class="row">
              <div class="col-md-6" v-for="(item, index) in category.items" :key="index">
                <div class="mb-3">
                  <h5 class="text-black mb-2">
                    <strong>{{item.name}}</strong>
                  </h5>
                  <div>
                    <p class="mb-2">
                      {{item.description}}
                    </p>
                    <a
                      :href="item.link"
                      target="_blank"
                      class="air__utils__link air__utils__link__underlined"
                    >
                      Examples
                      <small>
                        <i class="icmn-link ml-1" />
                      </small>
                    </a>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
import data from './data.json'

export default {
  data: function() {
    return {
      data,
    }
  },
}
</script>
