<template>
    <div>
        <h2>checkbox</h2>
        <div class="demo-block">
            <t-row :gutter="20">
                <t-col :span="8">
                    <t-checkbox label="label在右边"></t-checkbox>
                    <t-checkbox label="label在左边" :labelLeft=true></t-checkbox>
                </t-col>
            </t-row>
        </div>
        <checkbox-md></checkbox-md>
        <h2>checkbox Group</h2>
        <div class="demo-block">
            <t-row :gutter="20">
                <t-col :span="8">
                    <t-checkbox-group>
                        <t-checkbox label="北京" val="Beijing"></t-checkbox>
                        <t-checkbox label="上海" val="Shanghai"></t-checkbox>
                        <t-checkbox label="成都" val="Chengdu"></t-checkbox>
                    </t-checkbox-group>
                </t-col>
            </t-row>
        </div>
        <checkbox-group></checkbox-group>
        <h2>checkbox style</h2>
        <div class="demo-block">
            <t-row :gutter="20">
                <t-col :span="24">
                    <t-checkbox-group>
                        <t-checkbox label="默认" val="1"></t-checkbox>
                        <t-checkbox label="默认选中" :checked="true" val="2"></t-checkbox>
                        <t-checkbox label="禁用" :disabled="true" val="3"></t-checkbox>
                        <t-checkbox label="禁用并选用" :checked="true" :disabled="true" val="4"></t-checkbox>
                    </t-checkbox-group>
                </t-col>
            </t-row>
        </div>
        <checkbox-style></checkbox-style>
        <h2>checkbox indeterminate</h2>
        <div class="demo-block">
            <t-row :gutter="20">
                <t-col :span="24">
                    <t-checkbox-group :indeterminate="true">
                        <t-checkbox label="默认" val="1"></t-checkbox>
                        <t-checkbox label="默认选中" :checked="true" val="2"></t-checkbox>
                        <t-checkbox label="禁用" :disabled="true" val="3"></t-checkbox>
                        <t-checkbox label="禁用并选用" :checked="true" :disabled="true" val="4"></t-checkbox>
                    </t-checkbox-group>
                </t-col>
            </t-row>
        </div>
        <checkbox-indeterminate></checkbox-indeterminate>
        <h2>checkbox limit</h2>
        <div class="demo-block">
            <t-row :gutter="20">
                <t-col :span="24">
                    <t-checkbox-group :min="1" :max="3">
                        <t-checkbox label="西瓜" val='1'></t-checkbox>
                        <t-checkbox label="苹果" val='2'></t-checkbox>
                        <t-checkbox label="栗子" val='3'></t-checkbox>
                        <t-checkbox label="香蕉" val='4'></t-checkbox>
                    </t-checkbox-group>
                </t-col>
            </t-row>
        </div>
        <checkbox-limit></checkbox-limit>
        <h2>checkbox border</h2>
        <div class="demo-block">
            <t-row :gutter="20">
                <t-col :span="24">
                    <t-checkbox-group>
                        <t-checkbox label="北京" val='1' :outbox="true"></t-checkbox>
                        <t-checkbox label="上海" val='2' :outbox="true"></t-checkbox>
                        <t-checkbox label="成都" val='3' :outbox="true"></t-checkbox>
                        <t-checkbox label="广州" val='4' :outbox="true"></t-checkbox>
                    </t-checkbox-group>
                </t-col>
            </t-row>
        </div>
        <checkbox-border></checkbox-border>
    </div>
</template>
<script>
import CheckboxMd from '../documents/checkbox/checkbox.md'
import CheckboxGroup from '../documents/checkbox/checkboxGroup.md'
import CheckboxStyle from '../documents/checkbox/checkboxStyle.md'
import CheckboxIndeterminate from '../documents/checkbox/checkboxIndeterminate.md'
import CheckboxLimit from '../documents/checkbox/checkboxLimit.md'
import CheckboxBorder from '../documents/checkbox/checkboxBorder.md'
export default {
  components: {
    CheckboxMd,
    CheckboxGroup,
    CheckboxStyle,
    CheckboxIndeterminate,
    CheckboxLimit,
    CheckboxBorder
  }
}
</script>
