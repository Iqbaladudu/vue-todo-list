<template>
    <div>
        <input type="checkbox" name="item" id="todo-item"  :checked="isDone" checked="false"/>
        <label for="todo-item">{{label}}</label>
    </div>
</template>

<script>
export default {
    props: {
        label: {
            required: true,
            type: String,
        },
        done: {
            default: false,
            type: Boolean,
        },
    },
    data() {
        return {
            isDone: this.done
        };
    }
};
</script>