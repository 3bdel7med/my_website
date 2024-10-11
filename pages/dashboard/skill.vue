<script lang="ts">
import "https://cdn.jsdelivr.net/npm/bootstrap@5.0.2/dist/js/bootstrap.bundle.min.js";

definePageMeta({
  layout: "custom",
});
/*
import axios from "axios";
export default {
  data() {
    return {
      skill: {
        name: "",
        file: "",
      },
    };
  },
  methods: {
    addSkill() {
      axios
        .post("http://127.0.0.1:8000/skill/store", this.skill)
        .then((responce) => {});
    },
  },
};*/
</script>
<template>
  <div>
    <button
      class="btn btn-primary"
      data-bs-toggle="modal"
      data-bs-target="#exampleModal"
    >
      Add New Skill
    </button>

    <table class="table">
      <thead>
        <tr>
          <th scope="col">#</th>
          <th scope="col">First</th>
          <th scope="col">Last</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <th scope="row">1</th>
          <td>Mark</td>
          <td>Otto</td>
        </tr>
        <tr>
          <th scope="row">2</th>
          <td>Jacob</td>
          <td>Thornton</td>
        </tr>
      </tbody>
    </table>
    <div
      class="modal fade"
      id="exampleModal"
      tabindex="-1"
      aria-labelledby="exampleModalLabel"
      aria-hidden="true"
    >
      <div class="modal-dialog">
        <div class="modal-content">
          <form>
            <div class="modal-header">
              <h5 class="modal-title" id="exampleModalLabel">Add Skill</h5>
              <button
                type="button"
                class="btn-close"
                data-bs-dismiss="modal"
                aria-label="Close"
              ></button>
            </div>
            <div class="modal-body">
              <div class="row">
                <div class="col-6">
                  <input
                    class="form-control"
                    type="text"
                    placeholder="Default input"
                    aria-label="default input example"
                  />
                </div>
                <div class="col-6">
                  <input
                   
                    class="form-control"
                    type="file"
                    placeholder="Default input"
                    aria-label="default input example"
                  />
                </div>
              </div>
            </div>
            <div class="modal-footer">
              <button
                type="button"
                class="btn btn-secondary"
                data-bs-dismiss="modal"
              >
                Close
              </button>
              <button @click="addSkill" type="button" class="btn btn-primary">
                Save changes
              </button>
            </div>
          </form>
        </div>
      </div>
    </div>
  </div>
</template>

