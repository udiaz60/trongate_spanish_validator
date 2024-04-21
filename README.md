To use:
In controllers example: 
            $this->module('validation_helper_es');
           
            $this->validation_helper_es->set_rules('municipio', 'municipio', 'required|min_length[2]|max_length[255]');
            $this->validation_helper_es->set_rules('departamento_id', 'departamento', 'required');

            $result = $this->validation_helper_es->run();

IN VIEWS
<h1><?= $headline ?></h1>
<?= Modules::run('validator_helper_es/validation_errorssp') ?>
<div class="card">
