# biblioteca-programa-o

<div id="app">
  <div ui-view></div>
</div>
<img class="img-responsive" src="https://tiinside.com.br/wp-content/uploads/2020/05/cropped-loguinhoti512x512.png">
<nav class="navbar navbar-default">
    <div class="container-fluid">
    <!-- Brand and toggle get grouped for better mobile display -->
        <div class="navbar-header">
            <button type="button" class="navbar-toggle collapsed" data-toggle="collapse" data-target="#bs-example-navbar-collapse-1" aria-expanded="false">
        <span class="sr-only">Pesquiasdor navigation</span>
        <span class="icon-bar"></span>
        <span class="icon-bar"></span>
        <span class="icon-bar"></span>
      </button>
            <a class="navbar-brand" href="#">Menu 2021 - MPD;</a>
        </div>

        <!-- Collect the nav links, forms, and other content for toggling -->
        <div class="collapse navbar-collapse" id="bs-example-navbar-collapse-1">
            <ul class="nav navbar-nav">
                <li class="dropdown">
                    <a href="#" class="dropdown-toggle" data-toggle="dropdown" role="button" aria-haspopup="true" aria-expanded="false">Cadastro <span class="caret"></span></a>
                    <ul class="dropdown-menu">
                        <li><a href="#">Setores da Programação</a></li>
                        <li><a href="#">Projetos</a></li>
                        <li><a href="#">Bibliotecas de dados</a></li>
                        <li><a href="#">Projetos em javascript</a></li>
                        <li><a href="#">Projetos em Angular(js)</a></li>
                        <li><a href="#">Setor TI</a></li>
                        <li><a href="#">Projetos Estudos</a></li>
                        <li><a href="#">Bibliotecas </a></li>
                        <li><a href="#">Sites pesquisar</a></li>
                        <li><a href="#">Frameworks/ Linguagem</a></li>
                    </ul>
                </li>
            </ul>
        </div>
        <!-- /.navbar-collapse -->
    </div>
    <!-- /.container-fluid -->
</nav>
<section class="content">
    <div class="row">
        <div class="col-xs-12">
            <div class="box">
                <form name="form" (ngSubmit)="save()" #setor="ngForm">
                    <div class="box-header">
                        <div class="box-tools">
                            <div class="input-group">
                                <button type="submit" class="btn btn-sm btn-success" [disabled]="!setor.form.valid"><i name="save" id="save" class="glyphicon glyphicon-ok"></i>Salvar</button>
                                <button class="btn btn-sm btn-danger" (click)="cancel()"><i class="glyphicon glyphicon-remove"></i>Cancelar</button>
                            </div>
                        </div>
                    </div>
                    <div class="box box-primary">
                        <div class="box-header">
                            <h3 class="box-title">Informe os dados Operacionais:</h3>
                        </div>
                        <div class="form-group">
                            <input type="text" id="nameSetor" name="nameSetor" class="form-control" placeholder=" descrição do setor" maxlength="100" [(ngModel)]="model.descricao" #nameSetor="ngModel" required/>
                            <span [hidden]="nameSetor.valid || nameSetor.pristine" class="alert alert-danger">descrição do setor</span>
                            
                        </div>
                        <div class="form-group">
                            <input type="text" id="nameSetor" name="nameSetor" class="form-control" placeholder=" pesquisa programação" maxlength="100" [(ngModel)]="model.descricao" #nameSetor="ngModel" required/>
                            <span [hidden]="nameSetor.valid || nameSetor.pristine" class="alert alert-danger">setor de pesquisa de Programação</span>
                            
                        </div>
                        <div class="form-group">
                            <input type="text" id="nameSetor" name="nameSetor" class="form-control" placeholder=" setor linguagens" maxlength="100" [(ngModel)]="model.descricao" #nameSetor="ngModel" required/>
                            <span [hidden]="nameSetor.valid || nameSetor.pristine" class="alert alert-danger">setor de linguagens de Programação</span>
                            
                        </div>
                         <div class="input-group">
                                <button type="submit" class="btn btn-sm btn-success" [disabled]="!setor.form.valid"><i name="save" id="save" class="glyphicon glyphicon-ok"></i>Salvar</button>
                        <div class="box box-primary">
                        <div class="box-header">
                            <h3 class="box-title">Informe Setores Programação:</h3>
                        </div>
                        <div class="form-group">
                            <input type="text" id="nameSetor" name="nameSetor" class="form-control" placeholder=" descrição do setor" maxlength="100" [(ngModel)]="model.descricao" #nameSetor="ngModel" required/>
                            <span [hidden]="nameSetor.valid || nameSetor.pristine" class="alert alert-danger">descrição da Programação</span>
                            
                        </div>
                        <div class="form-group">
                            <input type="text" id="nameSetor" name="nameSetor" class="form-control" placeholder=" pesquisa python" maxlength="100" [(ngModel)]="model.descricao" #nameSetor="ngModel" required/>
                            <span [hidden]="nameSetor.valid || nameSetor.pristine" class="alert alert-danger"> pesquisar em Python</span>
                            
                        </div>
                        <div class="form-group">
                            <input type="text" id="nameSetor" name="nameSetor" class="form-control" placeholder=" setor angular" maxlength="100" [(ngModel)]="model.descricao" #nameSetor="ngModel" required/>
                            <span [hidden]="nameSetor.valid || nameSetor.pristine" class="alert alert-danger">pesquisar em Angular</span>
                            
                        </div>
                         <div class="input-group">
                                <button type="submit" class="btn btn-sm btn-success" [disabled]="!setor.form.valid"><i name="save" id="save" class="glyphicon glyphicon-ok"></i>Salvar</button>
                        <div class="box box-primary">
                        <div class="box-header">
                            <h3 class="box-title">Informe os Frameworks:</h3>
                        </div>
                        <div class="form-group">
                            <input type="text" id="nameSetor" name="nameSetor" class="form-control" placeholder=" descrição do angularjs" maxlength="100" [(ngModel)]="model.descricao" #nameSetor="ngModel" required/>
                            <span [hidden]="nameSetor.valid || nameSetor.pristine" class="alert alert-danger">descrição do Angularjs</span>
                            
                        </div>
                        <div class="form-group">
                            <input type="text" id="nameSetor" name="nameSetor" class="form-control" placeholder="descricao nodejs" maxlength="100" [(ngModel)]="model.descricao" #nameSetor="ngModel" required/>
                            <span [hidden]="nameSetor.valid || nameSetor.pristine" class="alert alert-danger">descrição Nodejs</span>
                            
                        </div>
                        
                        <div class="form-group">
                            <input type="text" id="nameSetor" name="nameSetor" class="form-control" placeholder="descricao V.Code" maxlength="100" [(ngModel)]="model.descricao" #nameSetor="ngModel" required/>
                            <span [hidden]="nameSetor.valid || nameSetor.pristine" class="alert alert-danger">descricao V. code</span>
                            
                        </div>
                         <div class="input-group">
                                <button type="submit" class="btn btn-sm btn-success" [disabled]="!setor.form.valid"><i name="save" id="save" class="glyphicon glyphicon-ok"></i>Salvar</button>

                    </div>
                    <div class="box-header">
                            <h3 class="box-title">Informe os Bancos de Dados:</h3>
                        </div>
                        <div class="form-group">
                            <input type="text" id="nameSetor" name="nameSetor" class="form-control" placeholder=" descrição do mysql" maxlength="100" [(ngModel)]="model.descricao" #nameSetor="ngModel" required/>
                            <span [hidden]="nameSetor.valid || nameSetor.pristine" class="alert alert-danger">Banco Mysql</span>
                            
                        </div>
                        <div class="form-group">
                            <input type="text" id="nameSetor" name="nameSetor" class="form-control" placeholder="descricao sql" maxlength="100" [(ngModel)]="model.descricao" #nameSetor="ngModel" required/>
                            <span [hidden]="nameSetor.valid || nameSetor.pristine" class="alert alert-danger">Banco Postgresql</span>
                            
                        </div>
                        
                        <div class="form-group">
                            <input type="text" id="nameSetor" name="nameSetor" class="form-control" placeholder="descricao oracle" maxlength="100" [(ngModel)]="model.descricao" #nameSetor="ngModel" required/>
                            <span [hidden]="nameSetor.valid || nameSetor.pristine" class="alert alert-danger">Banco Oracle SQL</span>
                            
                        </div>
                         <div class="input-group">
                                <button type="submit" class="btn btn-sm btn-success" [disabled]="!setor.form.valid"><i name="save" id="save" class="glyphicon glyphicon-ok"></i>Salvar</button>

                    </div>
                    <!-- /.box -->

                </form>
            </div>
        </div>
    </div>
</section>
