const { Router } = require("express");
const controllers  = require("../controllers/controller");


const { temp_middleware } = require("../middlewares/middleware");


const router = Router();

router.route("/").get(temp_middleware, controllers.basic_controller);



module.exports = router;
