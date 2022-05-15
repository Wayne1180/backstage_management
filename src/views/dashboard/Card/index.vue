<template>
  <div>
    <el-row :gutter="10">
      <el-col :span="6">
        <el-card>
          <!-- 第一个card -->
          <Detail title="总销售额" count="￥126560">
            <template slot="charts">
              <span
                >周同比&nbsp;&nbsp;56.67%
                <svg
                  t="1652540218860"
                  class="icon"
                  viewBox="0 0 1024 1024"
                  version="1.1"
                  xmlns="http://www.w3.org/2000/svg"
                  p-id="2814"
                  width="16"
                  height="16"
                >
                  <path
                    d="M768 384L512 128 256 384h192v512h128V384z"
                    p-id="2815"
                    fill="#d81e06"
                  ></path></svg
              ></span>
              &nbsp;&nbsp;
              <span
                >日同比&nbsp;&nbsp;19.96%<svg
                  t="1652540388058"
                  class="icon"
                  viewBox="0 0 1024 1024"
                  version="1.1"
                  xmlns="http://www.w3.org/2000/svg"
                  p-id="3826"
                  width="16"
                  height="16"
                >
                  <path
                    d="M768 640l-256 256-256-256h192V128h128v512z"
                    p-id="3827"
                    fill="#1afa29"
                  ></path></svg
              ></span>
            </template>
            <template slot="footer">
              <span>日销售额￥12423</span>
            </template>
          </Detail>
        </el-card>
      </el-col>
      <el-col :span="6">
        <el-card>
          <!-- 第二个card -->
          <Detail title="访问量" count="88460">
            <template slot="charts">
              <lineCharts> </lineCharts>
            </template>
            <template slot="footer">
              <span>日访问量 1234</span>
            </template>
          </Detail>
        </el-card>
      </el-col>
      <el-col :span="6">
        <el-card>
          <!-- 第三个card -->
          <Detail title="支付笔数" count="88460">
            <template slot="charts">
              <barCharts></barCharts>
            </template>
            <template slot="footer">
              <span>转换率64%</span>
            </template>
          </Detail>
        </el-card>
      </el-col>
      <el-col :span="6">
        <el-card>
          <!-- 第四个card -->
          <Detail title="运营活动效果" count="78%">
            <template slot="charts">
              <progressCharts></progressCharts>
            </template>
            <template slot="footer">
              <span
                >周同比&nbsp;&nbsp;12%
                <svg
                  t="1652540218860"
                  class="icon"
                  viewBox="0 0 1024 1024"
                  version="1.1"
                  xmlns="http://www.w3.org/2000/svg"
                  p-id="2814"
                  width="16"
                  height="16"
                >
                  <path
                    d="M768 384L512 128 256 384h192v512h128V384z"
                    p-id="2815"
                    fill="#d81e06"
                  ></path></svg
              ></span>
              &nbsp;&nbsp;
              <span
                >日同比&nbsp;&nbsp;11%<svg
                  t="1652540388058"
                  class="icon"
                  viewBox="0 0 1024 1024"
                  version="1.1"
                  xmlns="http://www.w3.org/2000/svg"
                  p-id="3826"
                  width="16"
                  height="16"
                >
                  <path
                    d="M768 640l-256 256-256-256h192V128h128v512z"
                    p-id="3827"
                    fill="#1afa29"
                  ></path></svg
              ></span>
            </template>
          </Detail>
        </el-card>
      </el-col>
    </el-row>
  </div>
</template>

<script>
import Detail from "./Detail";
import lineCharts from "./lineChart";
import barCharts from "./barCharts";
import progressCharts from "./progressCharts";
export default {
  name: "",
  components: {
    Detail,
    lineCharts,
    barCharts,
    progressCharts,
  },
};
</script>

<style>
</style>