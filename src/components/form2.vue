<!--
 * @Author: honghong
 * @Date: 2019-11-08 23:00:35
 * @LastEditors: honghong
 * @LastEditTime: 2019-11-09 09:29:28
 * @Description: 
 * @email: 3300536651@qq.com
 -->
<template>
  <div>
    <a-form>
      <a-form-item
        :label-col="labelCol"
        :wrapper-col="wrapperCol"
        label="名字"
        validate-status="error"
        help="Should be combination of numbers & alphabets"
      >
        <a-input id="error" placeholder="unavailable choice" />
      </a-form-item>

      <a-form-item
        :label-col="labelCol"
        :wrapper-col="wrapperCol"
        label="Warning"
        validate-status="warning"
      >
        <a-input id="warning" placeholder="Warning" />
      </a-form-item>

      <a-form-item
        :label-col="labelCol"
        :wrapper-col="wrapperCol"
        label="Validating"
        has-feedback
        validate-status="validating"
        help="The information is being validated..."
      >
        <a-input id="validating" placeholder="I'm the content is being validated" />
      </a-form-item>

      <a-form-item
        :label-col="labelCol"
        :wrapper-col="wrapperCol"
        label="Success"
        has-feedback
        validate-status="success"
      >
        <a-input id="success" placeholder="I'm the content" />
      </a-form-item>

      <a-form-item
        :label-col="labelCol"
        :wrapper-col="wrapperCol"
        label="Warning"
        has-feedback
        validate-status="warning"
      >
        <a-input id="warning2" placeholder="Warning" />
      </a-form-item>

      <a-form-item
        :label-col="labelCol"
        :wrapper-col="wrapperCol"
        label="Fail"
        has-feedback
        validate-status="error"
        help="Should be combination of numbers & alphabets"
      >
        <a-input id="error2" placeholder="unavailable choice" />
      </a-form-item>

      <a-form-item
        :label-col="labelCol"
        :wrapper-col="wrapperCol"
        label="Success"
        has-feedback
        validate-status="success"
      >
        <a-date-picker style="width: 100%" />
      </a-form-item>

      <a-form-item
        :label-col="labelCol"
        :wrapper-col="wrapperCol"
        label="Warning"
        has-feedback
        validate-status="warning"
      >
        <a-time-picker style="width: 100%" />
      </a-form-item>

      <a-form-item
        :label-col="labelCol"
        :wrapper-col="wrapperCol"
        label="Error"
        has-feedback
        validate-status="error"
      >
        <a-select default-value="1">
          <a-select-option value="1">Option 1</a-select-option>
          <a-select-option value="2">Option 2</a-select-option>
          <a-select-option value="3">Option 3</a-select-option>
        </a-select>
      </a-form-item>

      <a-form-item
        :label-col="labelCol"
        :wrapper-col="wrapperCol"
        label="Validating"
        has-feedback
        validate-status="validating"
        help="The information is being validated..."
      >
        <a-cascader :default-value="['1']" :options="[]" />
      </a-form-item>

      <a-form-item
        label="inline"
        :label-col="labelCol"
        :wrapper-col="wrapperCol"
        style="margin-bottom:0;"
      >
        <a-form-item
          validate-status="error"
          help="Please select the correct date"
          :style="{ display: 'inline-block', width: 'calc(50% - 12px)' }"
        >
          <a-date-picker style="width: 100%" />
        </a-form-item>
        <span :style="{ display: 'inline-block', width: '24px', textAlign: 'center' }">-</span>
        <a-form-item :style="{ display: 'inline-block', width: 'calc(50% - 12px)' }">
          <a-date-picker style="width: 100%" />
        </a-form-item>
      </a-form-item>

      <a-form-item
        :label-col="labelCol"
        :wrapper-col="wrapperCol"
        label="Success"
        has-feedback
        validate-status="success"
      >
        <a-input-number style="width: 100%" />
      </a-form-item>
    </a-form>
  </div>
</template> 

<script>
export default {
  name: "Form2",
  data() {
    return {
      labelCol: {
        xs: { span: 24 },
        sm: { span: 5 }
      },
      wrapperCol: {
        xs: { span: 24 },
        sm: { span: 12 }
      }
    };
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
