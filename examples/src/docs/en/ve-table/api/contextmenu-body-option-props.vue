<template>
    <div>
        <tpl
            :desc="desc"
            :anchor="anchor"
            :table-data="db.contextmenuBodyOption.data"
            :columns="db.contextmenuBodyOption.columns"
        />
    </div>
</template>
<script>
import tpl from "@/comp/api-tpl";
import { db } from "./db";
export default {
    components: { tpl },
    props: {
        anchor: {
            type: String,
            default: "Contextmenu option",
        },
        desc: {
            type: String,
            default: "contextmenuBodyOption",
        },
    },
    data() {
        return {
            db: db,
        };
    },
};
</script>
