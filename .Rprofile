if (interactive() && Sys.getenv("RSTUDIO") == "1") {
  if (requireNamespace("rstudioapi", quietly = TRUE)) {
    ctx <- rstudioapi::getActiveDocumentContext()
    if (!is.null(ctx$path)) {
      this_dir <- dirname(ctx$path)
      message("Setting working directory to: ", this_dir)
      try(setwd(this_dir), silent = TRUE)
    }
  }
}
