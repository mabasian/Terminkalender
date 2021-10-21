<template>
  <div id="app">
    <div id="calender-week">
      <div class="container-fluid mt-5">
        <div class="row">
          <div class="col-12">
            <div class="card-group">
              <!--Tage-->
              <div class="card">
                <div class="card-header text-center bg-vue">
                  <strong>Mohtag</strong>
                </div>
                <div class="card-body">
                  <div>1</div>
                  <div class="alert alert-success text-center">
                    <div>Müll rausbringen</div>
                    <div>
                      <i class="far fa-edit"></i>
                      <i class="far fa-trash-alt"></i>
                    </div>
                  </div>
                </div>
              </div>
              <div class="card">
                <div class="card-header text-center bg-vue">
                  <strong>Dienstag</strong>
                </div>
                <div class="card-body">
                  <div>2</div>
                </div>
              </div>
              <div class="card">
                <div class="card-header text-center bg-vue">
                  <strong>Mitwoch</strong>
                </div>
                <div class="card-body">
                  <div>3</div>
                </div>
              </div>
              <div class="card">
                <div class="card-header text-center bg-vue">
                  <strong>Donnerstag</strong>
                </div>
                <div class="card-body">
                  <div>4</div>
                </div>
              </div>
              <div class="card">
                <div class="card-header text-center bg-vue">
                  <strong>Freitag</strong>
                </div>
                <div class="card-body">
                  <div>5</div>
                  <div class="alert alert-success text-center">
                    <div>Müll rausbringen</div>
                    <div>
                      <i class="far fa-edit"></i>
                      <i class="far fa-trash-alt"></i>
                    </div>
                  </div>
                </div>
              </div>
              <div class="card">
                <div class="card-header text-center bg-vue">
                  <strong>Samstag</strong>
                </div>
                <div class="card-body">
                  <div>6</div>
                </div>
              </div>
              <div class="card">
                <div class="card-header text-center bg-vue">
                  <strong>Sonntag</strong>
                </div>
                <div class="card-body">
                  <div>7</div>
                  <div class="alert alert-primary text-center">
                    <div>Grillen mit Freunden</div>
                    <div>
                      <i class="far fa-edit"></i>
                      <i class="far fa-trash-alt"></i>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>

    <div id="calender-entry">
      <div class="container mt-5">
        <div class="row">
          <div class="col-6 offset-3">
            <div class="card">
              <div class="card-header text-center bg-vue2">
              <h5>Neuer Termin für: <strong>Dienstag</strong></h5>
              </div>
              <div class="card-body">
              <input 
              type="text"
              class="form-control"
              placeholder="Neuer Termin"
              >
              <div class="mt-3 text-center">
              <span
              v-for="(color,index) in ['primary','success','info','warning','danger']"
              :key="index"
              class="alert mr-2 square "
              :class="['alert-'+color]"
              style="cursor: pointer;"
              ></span>
              </div>
              <hr>
              <button class="btn btn-primary bg-vue btn-block">Eintragen</button>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "App",
};
</script>

<style scoped>
.bg-vue {
  background-color: #41b883;
  color: #34495e;
}
.bg-vue2 {
  background-color: #D3A9AB;
  color: #4a545e;
}
.square{
  width: 40px;
  height: 40px;
}
</style>
